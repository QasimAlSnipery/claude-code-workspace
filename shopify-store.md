# Shopify Store Connection

## Store Details

| Field            | Value                          |
|------------------|--------------------------------|
| Store Name       | My Store 3                     |
| Owner            | Mohammed Qarawlws              |
| Shopify Domain   | b05v6e-nh.myshopify.com        |
| Admin URL        | https://admin.shopify.com/store/b05v6e-nh |
| Plan             | Basic                          |
| Currency         | USD                            |
| Country          | United States (Wyoming)        |
| Timezone         | GMT+03:00 (Asia/Baghdad)       |
| Primary Location | 108195315896                   |
| API Version      | 2025-01                        |
| Created          | 2026-04-27                     |

## Credentials

Stored in `.env` (gitignored — never committed to GitHub):

```
SHOPIFY_STORE_DOMAIN=b05v6e-nh.myshopify.com
SHOPIFY_ACCESS_TOKEN=<see .env file>
SHOPIFY_API_VERSION=2025-01
```

## How to Query the Store

**REST example** (shop info):
```bash
curl -H "X-Shopify-Access-Token: <token>" \
     https://b05v6e-nh.myshopify.com/admin/api/2025-01/shop.json
```

**GraphQL endpoint**:
```
https://b05v6e-nh.myshopify.com/admin/api/2025-01/graphql.json
```

## Security Note

The access token (`shpat_...`) should be regenerated in Shopify Admin if it was ever shared in a chat or public place. Go to:
**Admin → Apps → Develop apps → Your app → API credentials → Regenerate**
