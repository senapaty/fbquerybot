# Meta Graph API Endpoints Reference

**Access Token:** `EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD`

**Quick Reference:**
- User ID: `122094735338961964`
- Ad Account: `act_12972328`
- WOW Club Page: `56878922808`
- Magical Journeys Page: `410130145739197`
- WOW Instagram: `17841402349285698`
- Business ID: `140572483644158`

---

## 📋 Table of Contents
1. [Token & User Info](#token--user-info)
2. [Facebook Pages](#facebook-pages)
3. [Instagram](#instagram)
4. [Ads & Campaigns](#ads--campaigns)
5. [Ad Insights & Analytics](#ad-insights--analytics)
6. [Business & Audiences](#business--audiences)
7. [Advanced Queries](#advanced-queries)

---

## 🔑 Token & User Info

### Check Token Validity & Permissions
```bash
curl -s "https://graph.facebook.com/v21.0/debug_token?input_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Current User Info
```bash
curl -s "https://graph.facebook.com/v21.0/me?access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### List All Pages/Accounts You Manage
```bash
curl -s "https://graph.facebook.com/v21.0/me/accounts?access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### List All Ad Accounts
```bash
curl -s "https://graph.facebook.com/v21.0/me/adaccounts?access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### List All Businesses
```bash
curl -s "https://graph.facebook.com/v21.0/me/businesses?fields=name,id,created_time&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

---

## 📘 Facebook Pages

### Get WOW Club Page Details
```bash
curl -s "https://graph.facebook.com/v21.0/56878922808?fields=name,category,category_list,fan_count,followers_count,link,website,about,description,phone,emails,instagram_business_account,cover,picture&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Magical Journeys Page Details
```bash
curl -s "https://graph.facebook.com/v21.0/410130145739197?fields=name,category,fan_count,followers_count,link,website,instagram_business_account&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Page Posts (Last 10)
```bash
# WOW Club posts
curl -s "https://graph.facebook.com/v21.0/56878922808/posts?fields=message,created_time,shares,reactions.summary(true),comments.summary(true),attachments,permalink_url,full_picture&limit=10&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Page Published Posts Only
```bash
curl -s "https://graph.facebook.com/v21.0/56878922808/published_posts?fields=message,created_time,shares,reactions.summary(true)&limit=20&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Page Feed (Including Posts from Others)
```bash
curl -s "https://graph.facebook.com/v21.0/56878922808/feed?fields=message,from,created_time,type&limit=10&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Page Videos
```bash
curl -s "https://graph.facebook.com/v21.0/56878922808/videos?fields=title,description,created_time,length,views,permalink_url&limit=10&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Page Photos/Albums
```bash
curl -s "https://graph.facebook.com/v21.0/56878922808/photos?fields=name,created_time,images,likes.summary(true)&limit=10&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Page Events
```bash
curl -s "https://graph.facebook.com/v21.0/56878922808/events?fields=name,description,start_time,end_time,place,attending_count&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Page Ratings/Reviews
```bash
curl -s "https://graph.facebook.com/v21.0/56878922808/ratings?fields=reviewer,rating,review_text,created_time&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Page Insights (Requires Page Access Token)
```bash
# Note: This requires page access token, not user token
# Get page token from /me/accounts endpoint first, then use it
curl -s "https://graph.facebook.com/v21.0/56878922808/insights?metric=page_impressions,page_engaged_users,page_post_engagements,page_fans&period=day&since=2026-01-01&until=2026-01-30&access_token=PAGE_ACCESS_TOKEN" | jq .
```

---

## 📸 Instagram

### Get Instagram Account Info
```bash
curl -s "https://graph.facebook.com/v21.0/17841402349285698?fields=username,name,biography,followers_count,follows_count,media_count,profile_picture_url,website&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Instagram Media/Posts (Last 20)
```bash
curl -s "https://graph.facebook.com/v21.0/17841402349285698/media?fields=id,caption,media_type,media_url,thumbnail_url,permalink,timestamp,like_count,comments_count,username&limit=20&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Instagram Stories (Active Stories Only)
```bash
curl -s "https://graph.facebook.com/v21.0/17841402349285698/stories?fields=id,media_type,media_url,permalink,timestamp&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Specific Instagram Post Details
```bash
# Replace MEDIA_ID with actual post ID (e.g., 17974224338827150)
curl -s "https://graph.facebook.com/v21.0/MEDIA_ID?fields=id,caption,media_type,media_url,thumbnail_url,permalink,timestamp,like_count,comments_count,children{media_url,media_type}&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Instagram Post Comments
```bash
curl -s "https://graph.facebook.com/v21.0/MEDIA_ID/comments?fields=text,username,timestamp,like_count&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Instagram Insights (Account Level)
```bash
# Last 30 days - reach and follower count
curl -s "https://graph.facebook.com/v21.0/17841402349285698/insights?metric=reach&metric_type=total_value&period=day&since=2026-01-01&until=2026-01-30&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Instagram Post Insights
```bash
# Replace MEDIA_ID with actual post ID
curl -s "https://graph.facebook.com/v21.0/MEDIA_ID/insights?metric=impressions,reach,engagement,saved,video_views&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Instagram Hashtag Search
```bash
curl -s "https://graph.facebook.com/v21.0/ig_hashtag_search?user_id=17841402349285698&q=wowclub&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

---

## 💰 Ads & Campaigns

### Get Ad Account Details
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328?fields=name,account_id,account_status,age,amount_spent,balance,currency,timezone_name,business,funding_source_details,min_campaign_group_spend_cap,spend_cap,created_time&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### List All Campaigns
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/campaigns?fields=name,status,objective,daily_budget,lifetime_budget,created_time,updated_time,start_time,stop_time,spend_cap&limit=50&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Active Campaigns Only
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/campaigns?fields=name,status,objective,daily_budget&filtering=[{\"field\":\"status\",\"operator\":\"IN\",\"value\":[\"ACTIVE\"]}]&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Specific Campaign Details
```bash
# Campaign ID: 6912083353056 (Sales - dubai - 30Jan)
curl -s "https://graph.facebook.com/v21.0/6912083353056?fields=name,status,objective,daily_budget,lifetime_budget,created_time,updated_time&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### List All Ad Sets
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/adsets?fields=name,status,campaign_id,daily_budget,lifetime_budget,bid_amount,billing_event,optimization_goal,targeting,created_time&limit=50&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Ad Sets for Specific Campaign
```bash
curl -s "https://graph.facebook.com/v21.0/6912083353056/adsets?fields=name,status,targeting,bid_amount,daily_budget,lifetime_budget,optimization_goal&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### List All Ads
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/ads?fields=name,status,effective_status,adset_id,campaign_id,created_time,updated_time,creative&limit=50&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Ads for Specific Ad Set
```bash
curl -s "https://graph.facebook.com/v21.0/6912083458056/ads?fields=name,status,creative&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Ad Creative Details
```bash
# Creative ID: 1415896356983085 (Dubai ad creative)
curl -s "https://graph.facebook.com/v21.0/1415896356983085?fields=id,name,title,body,object_story_spec,image_url,video_id,thumbnail_url,effective_object_story_id,link_url&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### List All Ad Creatives
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/adcreatives?fields=name,title,body,object_story_spec,image_url,thumbnail_url&limit=20&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Ad Images
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/adimages?fields=hash,url,name,width,height&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Ad Videos
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/advideos?fields=id,title,length,source,thumbnails&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

---

## 📊 Ad Insights & Analytics

### Ad Account Insights (Last 30 Days)
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/insights?fields=impressions,clicks,spend,reach,frequency,ctr,cpc,cpm,cpp,actions,action_values,conversions,cost_per_conversion&date_preset=last_30d&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Ad Account Insights (Custom Date Range)
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/insights?fields=impressions,clicks,spend,reach,ctr,cpc,cpm&time_range={'since':'2026-01-01','until':'2026-01-30'}&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Ad Account Insights (Daily Breakdown)
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/insights?fields=impressions,spend,reach,clicks&time_increment=1&date_preset=last_7d&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Campaign Insights
```bash
curl -s "https://graph.facebook.com/v21.0/6912083353056/insights?fields=impressions,clicks,spend,reach,ctr,cpc,cpm,actions,conversions&date_preset=last_30d&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Ad Set Insights
```bash
curl -s "https://graph.facebook.com/v21.0/6912083458056/insights?fields=impressions,clicks,spend,reach,ctr,cpc,actions&date_preset=last_7d&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Individual Ad Insights
```bash
# Ad ID: 6912083531856 (Solo Women's Dubai – Main Ad)
curl -s "https://graph.facebook.com/v21.0/6912083531856/insights?fields=impressions,clicks,spend,reach,ctr,cpc,cpm,actions,action_values,conversions&date_preset=lifetime&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Insights with Demographic Breakdown (Age & Gender)
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/insights?fields=impressions,spend,clicks&breakdowns=age,gender&date_preset=last_30d&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Insights by Placement (Facebook, Instagram, etc.)
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/insights?fields=impressions,spend,clicks&breakdowns=publisher_platform&date_preset=last_30d&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Insights by Device (Mobile, Desktop)
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/insights?fields=impressions,spend,clicks&breakdowns=device_platform&date_preset=last_30d&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Insights by Country
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/insights?fields=impressions,spend,clicks,reach&breakdowns=country&date_preset=last_30d&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get All Available Actions/Conversions
```bash
curl -s "https://graph.facebook.com/v21.0/6912083531856/insights?fields=actions,action_values,conversions,conversion_values,cost_per_action_type,cost_per_conversion&date_preset=lifetime&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

---

## 🏢 Business & Audiences

### Get Business Details
```bash
curl -s "https://graph.facebook.com/v21.0/140572483644158?fields=name,id,created_time,verification_status,profile_picture_uri&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Custom Audiences
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/customaudiences?fields=name,description,approximate_count_lower_bound,approximate_count_upper_bound,delivery_status,subtype,time_created,time_updated&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Saved Audiences
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/saved_audiences?fields=name,targeting,approximate_count&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Pixel Data (if available)
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/adspixels?fields=name,code,creation_time,last_fired_time&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Ad Account Activities (Audit Log)
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/activities?fields=event_type,event_time,extra_data&limit=20&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Conversion Tracking (if configured)
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/customconversions?fields=name,rule,event_source_type&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Catalog (if using Dynamic Ads)
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/product_catalogs?fields=name,product_count&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

---

## 🔍 Advanced Queries

### Search for Targeting Interests
```bash
curl -s "https://graph.facebook.com/v21.0/search?type=adinterest&q=travel&limit=10&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Delivery Estimate (Reach Estimate for Targeting)
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/delivery_estimate?optimization_goal=REACH&targeting_spec={'geo_locations':{'countries':['IN']},'age_min':18,'age_max':65}&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Minimum Budgets
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/minimum_budgets?bid_amount=5000&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Generate Ad Preview
```bash
# Get preview of ad creative
curl -s "https://graph.facebook.com/v21.0/1415896356983085/previews?ad_format=DESKTOP_FEED_STANDARD&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Campaign Optimization Suggestions
```bash
curl -s "https://graph.facebook.com/v21.0/6912083353056/recommendations?access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Export Ad Report (Async)
```bash
# Create async report
curl -X POST "https://graph.facebook.com/v21.0/act_12972328/insights?fields=campaign_name,impressions,clicks,spend&date_preset=last_30d&level=campaign&async=true&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD"

# Check report status (replace REPORT_ID)
curl -s "https://graph.facebook.com/v21.0/REPORT_ID?access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Compare Multiple Campaigns
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/insights?fields=campaign_id,campaign_name,impressions,clicks,spend,ctr,cpc&level=campaign&date_preset=last_30d&limit=10&sort=spend_descending&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

### Get Attribution Windows Data
```bash
curl -s "https://graph.facebook.com/v21.0/act_12972328/insights?fields=campaign_name,actions,action_attribution_windows&action_attribution_windows=['1d_click','7d_click','28d_click','1d_view','7d_view']&date_preset=last_30d&access_token=EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD" | jq .
```

---

## 📝 Useful Tips

### Save Output to File
```bash
curl -s "URL" | jq . > output.json
```

### Pretty Print Without jq
```bash
curl -s "URL"
```

### Use Environment Variable for Token
```bash
export FB_TOKEN="EAAYgVKcCK4oBPBH8XxdUZAZCgpDLT5pVGiCExK6tZBLJJnWT4kPRNeIXCbFbP9dsZAhLppvIrWQ242U2G1GR8dB9BA1894oa6dZBILnXsmWCVneZAm2pyc8V4cnbuXLElTtFMCM53OPeqZA8YCobq3QdhBtP8UxohHVSMAOCJc58ZCVjaCNtJGajNs5DueypSOcPugZDZD"

# Then use in commands
curl -s "https://graph.facebook.com/v21.0/me?access_token=$FB_TOKEN" | jq .
```

### Date Presets Available
- `today`, `yesterday`
- `this_week`, `last_week`
- `this_month`, `last_month`
- `last_7d`, `last_14d`, `last_30d`, `last_90d`
- `this_quarter`, `last_quarter`
- `this_year`, `last_year`
- `lifetime`

### Common Breakdowns
- `age`, `gender`
- `country`, `region`, `dma`
- `device_platform`, `publisher_platform`, `platform_position`
- `hourly_stats_aggregated_by_advertiser_time_zone`
- `product_id` (for catalog ads)

### Rate Limits
- Most endpoints: 200 calls per hour per user
- Marketing API: Based on ad spend
- Use batch requests to optimize

---

## 🔗 Official Documentation
- **Graph API Reference:** https://developers.facebook.com/docs/graph-api/reference/
- **Marketing API:** https://developers.facebook.com/docs/marketing-api/
- **Instagram Graph API:** https://developers.facebook.com/docs/instagram-api/

---

**Last Updated:** 2026-01-30
**API Version:** v21.0
