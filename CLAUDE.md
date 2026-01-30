# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Marketing Copilot - A unified analytics dashboard for e-commerce businesses managing Instagram/Facebook advertising and social media performance.

**Target Market**: Instagram/Facebook sellers running performance marketing campaigns
**Pricing**: $5/month initially
**Core Problem**: E-commerce owners struggle with scattered data sources (Meta ads, social insights) and difficulty understanding actionable insights from their data.

## Product Features

**V1 Scope**:
- Meta (Facebook/Instagram) OAuth integration for ads and social performance data
- Unified dashboard displaying ROAS, ad performance, and social engagement metrics
- ChatGPT-style natural language interface for querying marketing data
- Automated alerts for ROAS changes and performance shifts

**Out of Scope for V1**:
- TikTok integration
- Creative analysis
- Google Ads integration

## Technical Architecture

### Data Layer
- Pull selective fields from ~500 available Meta Marketing API columns
- Transform into standardized format for analysis
- Standard Shopify stores have pre-configured pixel setup for purchase tracking
- Handle rate limits, pagination, and scheduled data syncs

### Authentication
- OAuth 2.0 flow for Meta API connection
- Multi-client data separation (support multiple e-commerce clients with their own Meta accounts)
- Token storage and refresh strategy
- Meta app is verified and ready with credentials available

### LLM Integration (Akash's focus area)
- Combine traditional data analysis with LLM interface
- Enable natural language queries on marketing data
- Common query examples:
  - "How is my ROAS trending this week?"
  - "Which ad creative is performing best?"
  - "Why did my engagement drop yesterday?"

### Development Approach
- Start with Meta sandbox environment for testing
- Design partner available: contact managing 15 client Facebook accounts
- Focus on simple, focused solution vs comprehensive funded solutions

## Project Resources

- Trello Board: https://trello.com/b/cmjQtdng/marketing-copilot (managed via API)
- Meta app credentials: Available and verified
- GitHub Repository: git@github.com:senapaty/fbquerybot.git

---

## Meta API Integration Learnings

### Access Tokens and Accounts

We have access to **2 separate Meta Business accounts** with full API access:

#### 1. WOW Club (Travel Business)
- **App:** socialOS (App ID: 1724397811542922)
- **Token Type:** SYSTEM_USER (never expires)
- **User ID:** 122094735338961964
- **Business:** WOW Club (ID: 140572483644158)
- **Token:** `EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD`

**Ad Account:**
- **ID:** act_12972328
- **Name:** WOW Ads Account
- **Currency:** INR
- **Timezone:** Asia/Kolkata
- **Status:** Active

**Facebook Pages:**
1. The WOW Club - Women on Wanderlust (56878922808) - 258,201 followers
2. Magical Journeys (410130145739197) - 5 followers

**Instagram:**
- @the.wowclub (17841402349285698) - 36,417 followers, 1,780 posts

**Campaigns:** 25+ campaigns (active: "Sales - dubai - 30Jan")

**Performance Summary (Last 37 months):**
- Impressions: 1
- Spend: ₹0
- Note: Limited recent activity

---

#### 2. Complement Theory Technologies
- **App:** n8nauto (App ID: 1261703592111781)
- **Token Type:** SYSTEM_USER (never expires)
- **User ID:** 122119745361064495
- **Business:** Complement Theory Technologies Pvt Ltd (ID: 447910974394269)
- **Token:** `EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD`

**Ad Accounts (5 total):**
1. **CT ad ac1** (act_463989343055629) - PRIMARY - Most Active
   - Currency: INR, Timezone: Asia/Kolkata
   - Performance (37 months):
     - Impressions: 183,453
     - Clicks: 6,062
     - Spend: ₹745,262.93
     - CTR: 3.30%
     - CPC: ₹122.94
     - Reach: 107,171

2. **CT ad ac2** (act_527537576376081) - Inactive
   - Currency: INR, Timezone: Asia/Kolkata

3. **CT ad ac3** (act_1581594466112579) - Inactive
   - Currency: INR, Timezone: Asia/Kolkata

4. **CT Ad ac4-US** (act_1096405025859740) - SECONDARY - Active
   - Currency: INR, Timezone: America/New_York
   - Performance (37 months):
     - Impressions: 37,096
     - Clicks: 756
     - Spend: ₹149,948.80
     - CTR: 2.04%
     - CPC: ₹198.34
     - Reach: 29,514

5. **CT ad ac5 - US and USD** (act_1364598024809245) - Disabled
   - Currency: USD, Timezone: America/New_York
   - Status: Account disabled

**Combined CT Performance (All Active Accounts):**
- Total Impressions: 220,549
- Total Clicks: 6,818
- Total Spend: ₹895,211.73
- Total Reach: 136,685
- Average CTR: 2.67%
- Average CPC: ₹131.30

---

### API Documentation Files

All curl commands and API references are documented in:
1. **`meta-api-endpoints.md`** - Complete WOW Club Meta API reference
2. **`Ct_ad_data.md`** - Complete Complement Theory Meta API reference

---

### Key API Learnings

#### 1. Maximum Data Retention
- **Facebook API Limitation:** Maximum lookback is **37 months** (~3 years)
- Cannot query data older than 37 months from current date
- Error code 3018 if attempting to go beyond this limit
- For historical data beyond 37 months, need to export reports regularly

#### 2. Token Permissions
Both tokens have comprehensive permissions including:
- `ads_management`, `ads_read` - Full ads access
- `business_management` - Business settings
- `pages_show_list`, `pages_read_engagement`, `pages_manage_posts`
- `instagram_basic`, `instagram_manage_insights`, `instagram_content_publish`
- `read_insights`, `attribution_read` - Analytics access
- `leads_retrieval` - Lead forms data

#### 3. API Endpoints Structure

**Base URL:** `https://graph.facebook.com/v21.0/`

**Key Endpoints:**
- `/me` - Current user info
- `/me/accounts` - Pages managed by user
- `/me/adaccounts` - Ad accounts accessible
- `/act_{ad-account-id}/campaigns` - List campaigns
- `/act_{ad-account-id}/adsets` - List ad sets
- `/act_{ad-account-id}/ads` - List ads
- `/act_{ad-account-id}/insights` - Performance insights
- `/act_{ad-account-id}/adcreatives` - Ad creatives
- `/{page-id}/posts` - Page posts
- `/{ig-account-id}/media` - Instagram posts
- `/{ig-account-id}/stories` - Instagram stories

#### 4. Insights Parameters

**Time Range:**
```bash
# URL encoded: %7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D
time_range={"since":"2022-12-30","until":"2026-01-30"}
```

**Date Presets:**
- `today`, `yesterday`
- `last_7d`, `last_14d`, `last_30d`, `last_90d`
- `this_month`, `last_month`
- `this_quarter`, `last_quarter`
- `lifetime`

**Levels:**
- `account` - Ad account level
- `campaign` - Campaign level
- `adset` - Ad set level
- `ad` - Individual ad level

**Breakdowns:**
- `age`, `gender` - Demographics
- `country`, `region` - Geography
- `device_platform` - Mobile/Desktop/Tablet
- `publisher_platform`, `platform_position` - Placement
- `hourly_stats_aggregated_by_advertiser_time_zone` - Hourly

**Key Metrics:**
- `impressions`, `reach`, `frequency`
- `clicks`, `ctr`, `cpc`, `cpm`, `cpp`
- `spend`, `actions`, `conversions`
- `cost_per_action_type`, `cost_per_conversion`
- `inline_link_clicks`, `inline_link_click_ctr`
- `video_play_actions`, `video_p25/p50/p75/p100_watched_actions`

#### 5. Pagination
- Most endpoints return paginated results
- Use `limit` parameter (max varies by endpoint, typically 25-500)
- Response includes `paging.next` URL for next page
- Response includes `paging.cursors` for before/after navigation

#### 6. Rate Limits
- Standard endpoints: 200 calls per hour per user
- Marketing API: Based on ad spend tier
- Use batch requests to optimize
- Implement exponential backoff for rate limit errors

---

### Common Query Patterns

#### Get All Campaigns with Performance
```bash
curl -s "https://graph.facebook.com/v21.0/act_{account-id}/insights?fields=campaign_id,campaign_name,impressions,clicks,spend,reach,ctr,cpc,actions&level=campaign&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&access_token={token}" | jq .
```

#### Get Top Performing Ads
```bash
curl -s "https://graph.facebook.com/v21.0/act_{account-id}/insights?fields=ad_id,ad_name,impressions,clicks,spend,ctr,cpc&level=ad&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&sort=spend_descending&limit=50&access_token={token}" | jq .
```

#### Get Demographics Breakdown
```bash
curl -s "https://graph.facebook.com/v21.0/act_{account-id}/insights?fields=impressions,clicks,spend,reach&breakdowns=age,gender&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&access_token={token}" | jq .
```

#### Get Daily Performance Trend
```bash
curl -s "https://graph.facebook.com/v21.0/act_{account-id}/insights?fields=impressions,spend,clicks,ctr&time_increment=1&date_preset=last_30d&access_token={token}" | jq .
```

---

### Data Architecture Recommendations

#### 1. Data Collection Strategy
- **Initial Sync:** Pull maximum 37 months of historical data
- **Ongoing Sync:** Daily incremental updates
- **Sync Schedule:**
  - Account/Campaign level: Daily at midnight
  - Ad level: Every 6 hours for active campaigns
  - Creative data: On campaign create/update

#### 2. Data Storage Schema
```
accounts/
  - account_id
  - name, currency, timezone, status
  - business_id, business_name

campaigns/
  - campaign_id, account_id
  - name, objective, status
  - budget (daily/lifetime)
  - start_time, stop_time

adsets/
  - adset_id, campaign_id
  - name, status
  - targeting (JSON)
  - bid_amount, optimization_goal

ads/
  - ad_id, adset_id
  - name, status
  - creative_id

insights_daily/
  - date, ad_id (or adset_id/campaign_id/account_id)
  - impressions, clicks, spend, reach, frequency
  - ctr, cpc, cpm
  - actions (JSON), conversions (JSON)

insights_breakdown/
  - date, ad_id, breakdown_type, breakdown_value
  - metrics (same as above)
```

#### 3. LLM Integration Points

**User Query Examples:**
1. "What's my ROAS for the last 7 days?"
   - Query: Account-level insights with actions/conversions, last_7d
   - Calculate: (Revenue from conversions) / spend

2. "Which campaigns performed best this month?"
   - Query: Campaign-level insights, this_month, sorted by ROAS or spend
   - Return: Top 5 campaigns with key metrics

3. "Show me age demographics for my top ad"
   - Query: Ad-level insights with age/gender breakdown
   - Filter: Top ad by spend or conversions
   - Visualize: Age distribution chart

4. "Why did my engagement drop yesterday?"
   - Query: Daily insights for yesterday vs last week same day
   - Compare: Frequency, placement, audience metrics
   - Suggest: Possible reasons based on data changes

**LLM Prompt Engineering:**
- Provide schema context to LLM
- Convert natural language to API parameters
- Handle metric calculations (ROAS, CTR, etc.)
- Generate insights from data patterns
- Suggest optimizations based on benchmarks

---

### Next Steps for Implementation

1. **Authentication Setup:**
   - Implement OAuth flow for user's Meta accounts
   - Store and refresh access tokens securely
   - Handle multi-account scenarios

2. **Data Pipeline:**
   - Build scheduled sync jobs (daily/hourly)
   - Implement pagination handling
   - Add rate limit retry logic
   - Store data in PostgreSQL or similar

3. **LLM Interface:**
   - Design prompt templates for common queries
   - Build query-to-API parameter mapping
   - Implement metric calculations
   - Create visualization helpers

4. **Testing:**
   - Use Meta sandbox environment
   - Test with design partner's 15 client accounts
   - Validate data accuracy vs Meta Ads Manager

5. **Optimization:**
   - Cache frequently accessed data
   - Batch API requests where possible
   - Pre-calculate common metrics
   - Index database appropriately

---

## References

- [Meta Marketing API Documentation](https://developers.facebook.com/docs/marketing-api/)
- [Meta Graph API Reference](https://developers.facebook.com/docs/graph-api/reference/)
- [Instagram Graph API](https://developers.facebook.com/docs/instagram-api/)
- Complete curl commands: See `meta-api-endpoints.md` and `Ct_ad_data.md`
