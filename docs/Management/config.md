---
sidebar_position: 2
description: Example config file
---

# Configuration File

---

```yaml title="config.yml"
Settings:
  Token: "BOT-TOKEN"
  Prefix: "-"
  Storage: "database.db"
  DevMode: false # This option will reset every addon configs.

Embeds:
  Color: "2f3136"

Branding:
  Name: "BrayanBot"
  Logo: "https://avatars.githubusercontent.com/u/99198112?s=200&v=4"
  Link: "https://brayanbot.dev"

WebServer:
  Enabled: true
  Port: 80
  Favicon: "favicon.ico"
  EndPoints:
    - Type: "URL"
      EndPoint: "/"
      URL: "https://brayanbot.dev/"

    - Type: "URL"
      EndPoint: "/discord"
      URL: "https://brayanbot.dev/discord"

    - Type: "Page"
      EndPoint: "/view/page"
      File: "assets/viewThisPage.html"

    - Type: "File"
      EndPoint: "/download"
      File: "assets/download.txt"
  Ratelimit:
    # It's recommended to keep this enabled.
    Enabled: true
    # Max Requests can be made per 1 minute
    MaxRequests: 1
    # IPs included will bypass Rate Limiting
    BypassIPs:
      - "127.0.0.1" # http://localhost/ | http://127.0.0.1/
```
