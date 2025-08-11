===
steps:

[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/lll9p/keepalive)

then:


Add `d1` database (name=DB database_name=keeper_d1) and copy `database_id`(`UUID`) to `wrangler.jsonc`

Add `API_CONFIGS` on worker's env:

```json
[
  {
    "apiKey": "AIzaSyCNUGhuoAvvaSJ2ypsqzgtuCaLSusRZs5Y",
    "apiName": "gemini-2.0-flash",
    "name": "Render",
    "url": "https://mygemini-balance.com/openai/v1/chat/completions",
  },
  {
    "apiKey": "AIzaSyDIlXo2EBB798zw6gt8AGiAMpF4noLSv6I",
    "apiName": "gemini-2.0-flash",
    "name": "WHAT",
    "url": "https://other-gemini-load/openai/v1/chat/completions",
  }
]
```


Add `QUESTIONS` on worker's env:

```json
["xxxxx1", "xxxxxxx2", "xxxxxxx3", "xxxxxxx4"]
```

