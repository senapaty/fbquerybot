# Complement Theory Ad Data - Complete API Reference

**Company:** Complement Theory Technologies Pvt Ltd
**Business ID:** 447910974394269
**Access Token:** `EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD`

**Date Range:** Maximum allowed (37 months) - 2022-12-30 to 2026-01-30

---

## 📋 Ad Accounts Overview

| Account Name | Account ID | Status | Currency | Timezone |
|--------------|------------|--------|----------|----------|
| CT ad ac1 | act_463989343055629 | Active | INR | Asia/Kolkata |
| CT ad ac2 | act_527537576376081 | Active | INR | Asia/Kolkata |
| CT ad ac3 | act_1581594466112579 | Active | INR | Asia/Kolkata |
| CT Ad ac4-US | act_1096405025859740 | Active | INR | America/New_York |
| CT ad ac5 - US and USD | act_1364598024809245 | Disabled | USD | America/New_York |

---

## 🎯 Ad Account Level Insights (37 Months)

### Get All Ad Account Insights - Comprehensive
```bash
# CT ad ac1 (PRIMARY - Most Active)
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?fields=impressions,clicks,spend,reach,frequency,ctr,cpc,cpm,cpp,actions,action_values,conversions,conversion_values,cost_per_action_type,cost_per_conversion,website_ctr,inline_link_clicks,inline_link_click_ctr,cost_per_inline_link_click,cost_per_unique_click,unique_clicks,unique_ctr&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT ad ac2
curl -s "https://graph.facebook.com/v21.0/act_527537576376081/insights?fields=impressions,clicks,spend,reach,frequency,ctr,cpc,cpm,cpp,actions,action_values,conversions,cost_per_conversion&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT ad ac3
curl -s "https://graph.facebook.com/v21.0/act_1581594466112579/insights?fields=impressions,clicks,spend,reach,frequency,ctr,cpc,cpm,cpp,actions,action_values,conversions,cost_per_conversion&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT Ad ac4-US
curl -s "https://graph.facebook.com/v21.0/act_1096405025859740/insights?fields=impressions,clicks,spend,reach,frequency,ctr,cpc,cpm,cpp,actions,action_values,conversions,cost_per_conversion&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT ad ac5 - US and USD (Disabled but may have historical data)
curl -s "https://graph.facebook.com/v21.0/act_1364598024809245/insights?fields=impressions,clicks,spend,reach,frequency,ctr,cpc,cpm,cpp,actions,action_values,conversions,cost_per_conversion&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

### Ad Account Insights - Daily Breakdown (Last 90 Days)
```bash
# CT ad ac1 - Daily breakdown
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?fields=impressions,clicks,spend,reach,ctr,cpc&time_increment=1&date_preset=last_90d&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT Ad ac4-US - Daily breakdown
curl -s "https://graph.facebook.com/v21.0/act_1096405025859740/insights?fields=impressions,clicks,spend,reach,ctr,cpc&time_increment=1&date_preset=last_90d&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

---

## 📢 Campaign Level Data

### List All Campaigns (All Accounts)
```bash
# CT ad ac1 - All campaigns
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/campaigns?fields=name,status,objective,daily_budget,lifetime_budget,created_time,updated_time,start_time,stop_time,spend_cap,configured_status,effective_status&limit=100&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT ad ac2 - All campaigns
curl -s "https://graph.facebook.com/v21.0/act_527537576376081/campaigns?fields=name,status,objective,daily_budget,lifetime_budget,created_time,updated_time&limit=100&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT ad ac3 - All campaigns
curl -s "https://graph.facebook.com/v21.0/act_1581594466112579/campaigns?fields=name,status,objective,daily_budget,lifetime_budget,created_time,updated_time&limit=100&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT Ad ac4-US - All campaigns
curl -s "https://graph.facebook.com/v21.0/act_1096405025859740/campaigns?fields=name,status,objective,daily_budget,lifetime_budget,created_time,updated_time&limit=100&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT ad ac5 - All campaigns
curl -s "https://graph.facebook.com/v21.0/act_1364598024809245/campaigns?fields=name,status,objective,daily_budget,lifetime_budget,created_time,updated_time&limit=100&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

### Campaign Insights - All Time (37 Months)
```bash
# CT ad ac1 - Campaign level insights
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?fields=campaign_id,campaign_name,impressions,clicks,spend,reach,ctr,cpc,cpm,actions,conversions&level=campaign&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&limit=100&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT Ad ac4-US - Campaign level insights
curl -s "https://graph.facebook.com/v21.0/act_1096405025859740/insights?fields=campaign_id,campaign_name,impressions,clicks,spend,reach,ctr,cpc,cpm,actions,conversions&level=campaign&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&limit=100&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

### Campaign Insights - Sorted by Spend (Top Performers)
```bash
# CT ad ac1 - Top campaigns by spend
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?fields=campaign_id,campaign_name,impressions,clicks,spend,reach,ctr,cpc,cpm&level=campaign&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&sort=spend_descending&limit=50&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

---

## 🎨 Ad Set Level Data

### List All Ad Sets
```bash
# CT ad ac1 - All ad sets
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/adsets?fields=name,status,campaign_id,daily_budget,lifetime_budget,bid_amount,billing_event,optimization_goal,targeting,created_time,updated_time,start_time,end_time,configured_status,effective_status&limit=100&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT Ad ac4-US - All ad sets
curl -s "https://graph.facebook.com/v21.0/act_1096405025859740/adsets?fields=name,status,campaign_id,daily_budget,lifetime_budget,bid_amount,billing_event,optimization_goal,targeting,created_time,updated_time&limit=100&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

### Ad Set Insights - All Time (37 Months)
```bash
# CT ad ac1 - Ad set level insights
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?fields=adset_id,adset_name,campaign_id,campaign_name,impressions,clicks,spend,reach,ctr,cpc,cpm,actions,conversions&level=adset&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&limit=200&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT Ad ac4-US - Ad set level insights
curl -s "https://graph.facebook.com/v21.0/act_1096405025859740/insights?fields=adset_id,adset_name,campaign_id,campaign_name,impressions,clicks,spend,reach,ctr,cpc,cpm,actions,conversions&level=adset&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&limit=200&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

---

## 🎯 Individual Ad Level Data

### List All Ads
```bash
# CT ad ac1 - All ads
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/ads?fields=name,status,adset_id,campaign_id,created_time,updated_time,creative,configured_status,effective_status,tracking_specs,conversion_specs&limit=200&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT Ad ac4-US - All ads
curl -s "https://graph.facebook.com/v21.0/act_1096405025859740/ads?fields=name,status,adset_id,campaign_id,created_time,updated_time,creative,configured_status,effective_status&limit=200&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

### Individual Ad Insights - All Time (37 Months)
```bash
# CT ad ac1 - Ad level insights
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?fields=ad_id,ad_name,adset_id,adset_name,campaign_id,campaign_name,impressions,clicks,spend,reach,frequency,ctr,cpc,cpm,actions,conversions,cost_per_action_type,cost_per_conversion,inline_link_clicks,inline_link_click_ctr,cost_per_inline_link_click&level=ad&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&limit=500&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT Ad ac4-US - Ad level insights
curl -s "https://graph.facebook.com/v21.0/act_1096405025859740/insights?fields=ad_id,ad_name,adset_id,adset_name,campaign_id,campaign_name,impressions,clicks,spend,reach,frequency,ctr,cpc,cpm,actions,conversions,cost_per_action_type,cost_per_conversion&level=ad&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&limit=500&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

### Individual Ad Insights - Sorted by Performance
```bash
# CT ad ac1 - Top ads by spend
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?fields=ad_id,ad_name,impressions,clicks,spend,reach,ctr,cpc,cpm&level=ad&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&sort=spend_descending&limit=100&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT ad ac1 - Top ads by CTR
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?fields=ad_id,ad_name,impressions,clicks,spend,reach,ctr,cpc,cpm&level=ad&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&sort=ctr_descending&limit=100&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

---

## 🎨 Ad Creative Data

### List All Ad Creatives
```bash
# CT ad ac1 - All ad creatives
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/adcreatives?fields=id,name,title,body,object_story_spec,image_url,video_id,thumbnail_url,effective_object_story_id,link_url,call_to_action_type,object_type,status&limit=200&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT Ad ac4-US - All ad creatives
curl -s "https://graph.facebook.com/v21.0/act_1096405025859740/adcreatives?fields=id,name,title,body,object_story_spec,image_url,video_id,thumbnail_url,effective_object_story_id,link_url&limit=200&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

### Get All Ad Images
```bash
# CT ad ac1 - All ad images
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/adimages?fields=hash,url,name,width,height,created_time&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT Ad ac4-US - All ad images
curl -s "https://graph.facebook.com/v21.0/act_1096405025859740/adimages?fields=hash,url,name,width,height&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

### Get All Ad Videos
```bash
# CT ad ac1 - All ad videos
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/advideos?fields=id,title,description,length,source,thumbnails,created_time&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

---

## 📊 Advanced Insights & Breakdowns

### Demographics Breakdown (Age & Gender)
```bash
# CT ad ac1 - Age and gender breakdown
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?fields=impressions,clicks,spend,reach,ctr,cpc&breakdowns=age,gender&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT Ad ac4-US - Age and gender breakdown
curl -s "https://graph.facebook.com/v21.0/act_1096405025859740/insights?fields=impressions,clicks,spend,reach,ctr,cpc&breakdowns=age,gender&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

### Placement Breakdown (Facebook, Instagram, Audience Network)
```bash
# CT ad ac1 - Placement breakdown
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?fields=impressions,clicks,spend,reach,ctr,cpc,cpm&breakdowns=publisher_platform,platform_position&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

### Device Breakdown (Mobile, Desktop, Tablet)
```bash
# CT ad ac1 - Device breakdown
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?fields=impressions,clicks,spend,reach,ctr,cpc&breakdowns=device_platform&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

### Geographic Breakdown (Country, Region)
```bash
# CT ad ac1 - Country breakdown
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?fields=impressions,clicks,spend,reach,ctr,cpc&breakdowns=country&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT ad ac1 - Region breakdown (India specific)
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?fields=impressions,clicks,spend,reach,ctr,cpc&breakdowns=region&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

---

## 📈 Conversion & Action Data

### All Actions and Conversions
```bash
# CT ad ac1 - All actions breakdown
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?fields=ad_id,ad_name,actions,action_values,conversions,conversion_values,cost_per_action_type,cost_per_conversion,website_ctr,outbound_clicks,outbound_clicks_ctr,cost_per_outbound_click&level=ad&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&limit=500&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

### Video Actions (If Video Ads)
```bash
# CT ad ac1 - Video engagement metrics
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?fields=ad_id,ad_name,video_play_actions,video_avg_time_watched_actions,video_p25_watched_actions,video_p50_watched_actions,video_p75_watched_actions,video_p100_watched_actions&level=ad&time_range=%7B%22since%22%3A%222022-12-30%22%2C%22until%22%3A%222026-01-30%22%7D&limit=500&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

---

## 🎯 Audiences & Targeting

### Custom Audiences
```bash
# CT ad ac1 - All custom audiences
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/customaudiences?fields=name,description,approximate_count_lower_bound,approximate_count_upper_bound,delivery_status,subtype,time_created,time_updated,operation_status&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT Ad ac4-US - All custom audiences
curl -s "https://graph.facebook.com/v21.0/act_1096405025859740/customaudiences?fields=name,description,approximate_count_lower_bound,approximate_count_upper_bound,delivery_status,subtype,time_created,time_updated&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

### Saved Audiences
```bash
# CT ad ac1 - All saved audiences
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/saved_audiences?fields=name,targeting,approximate_count,time_created,time_updated&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

---

## 🔍 Audit & Activity Logs

### Ad Account Activities (Last 100 Events)
```bash
# CT ad ac1 - Activity log
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/activities?fields=event_type,event_time,extra_data&limit=100&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

```bash
# CT Ad ac4-US - Activity log
curl -s "https://graph.facebook.com/v21.0/act_1096405025859740/activities?fields=event_type,event_time,extra_data&limit=100&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

---

## 📱 Pixels & Tracking

### Ad Pixels
```bash
# CT ad ac1 - All pixels
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/adspixels?fields=name,code,creation_time,last_fired_time,is_created_by_business,is_unavailable&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

### Custom Conversions
```bash
# CT ad ac1 - All custom conversions
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/customconversions?fields=name,rule,event_source_type,custom_event_type&access_token=EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD" | jq .
```

---

## 💡 Tips & Best Practices

### Save Results to File
```bash
# Save to JSON file
curl -s "URL" | jq . > ct_ad_data_$(date +%Y%m%d).json
```

### Environment Variable for Token
```bash
export CT_TOKEN="EAAR7g0JrbqUBQnFdV9RzwsEUc6GvKGxS4RY70bx7ogSF4wsHzijZAaOZCwOgsYRu9Is7qY8qMyx67ZCM79lyihG1R8N1FWioiWsYHOMxbRHq0EVGl2YnyPydaHWL9BqWiIy3HTBVI77JHE0enK5xPZCpNp7BoHddwFEfqmJJ0VyfLBP2bOX0PB3dGWSX6ieuNQZDZD"

# Then use in commands
curl -s "https://graph.facebook.com/v21.0/act_463989343055629/insights?...&access_token=$CT_TOKEN" | jq .
```

### Pagination
Most endpoints return paginated results. Use the `paging.next` URL from the response to get the next page:
```bash
# After first request, check response for paging.next
# Then use that URL directly
curl -s "PAGING_NEXT_URL" | jq .
```

### Rate Limits
- Marketing API rate limits are based on ad spend
- If you hit rate limits, implement exponential backoff
- Use batch requests to optimize API calls

---

## 📊 Key Insights Summary (37 Months)

Based on the data pulled:

### Active Accounts Performance:
1. **CT ad ac1 (act_463989343055629)** - PRIMARY ACCOUNT
   - Impressions: 183,453
   - Clicks: 6,062
   - Spend: ₹745,262.93
   - CTR: 3.30%
   - CPC: ₹122.94

2. **CT Ad ac4-US (act_1096405025859740)** - SECONDARY ACCOUNT
   - Impressions: 37,096
   - Clicks: 756
   - Spend: ₹149,948.80
   - CTR: 2.04%
   - CPC: ₹198.34

### Recommendations:
- Focus on CT ad ac1 as it shows better performance
- Analyze top-performing ads and replicate successful strategies
- Review inactive accounts (ac2, ac3, ac5) for potential reactivation
- Deep dive into demographic and placement breakdowns for optimization

---

**Last Updated:** 2026-01-30
**API Version:** v21.0
**Data Range:** 2022-12-30 to 2026-01-30 (37 months)
