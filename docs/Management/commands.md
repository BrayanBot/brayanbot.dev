---
sidebar_position: 3
description: Example Commands File
---

# Commands File

---

```yaml title="lang.yml"
DisabledCommands: []
General:
  Help:
    Description: "Displays all Bot Commands"
    Usage: "help"
    Aliases: []
    Permission:
      - "@everyone"
    AllowedChannels: false
    DeleteCommand: false
    SlashCommand:
      Enabled: true
      Data:
        Name: help
        Description: "Displays all Bot Commands"
        Options:
          - Type: "string"
            Name: "command"
            Description: "Command for info"
  Ping:
    Description: "Displays Bot Pings"
    Usage: "ping"
    Aliases: []
    Permission:
      - "@everyone"
    AllowedChannels: false
    DeleteCommand: false
    SlashCommand:
      Enabled: true
      Data:
        Name: ping
        Description: "Displays Bot Pings"
  Uptime:
    Description: "View Your Bot's Current Uptime"
    Usage: "uptime"
    Aliases: []
    Permission:
      - "@everyone"
    AllowedChannels: false
    DeleteCommand: false
    SlashCommand:
      Enabled: true
      Data:
        Name: uptime
        Description: "View Your Bot's Current Uptime"
  ServerInfo:
    Description: "View Server's Information"
    Usage: "serverinfo"
    Aliases:
      - "guildinfo"
    Permission:
      - "@everyone"
    AllowedChannels: false
    DeleteCommand: false
    SlashCommand:
      Enabled: true
      Data:
        Name: serverinfo
        Description: "View Server's Information"
  Avatar:
    Description: "Displays user's avatar"
    Usage: "avatar <user>"
    Aliases:
      - "av"
    Permission:
      - "@everyone"
    AllowedChannels: false
    DeleteCommand: false
    SlashCommand:
      Enabled: true
      Data:
        Name: avatar
        Description: "Displays user's avatar"
        Options:
          - Type: "User"
            Name: "target"
            Description: "User Mention"
Admin:
  Eval:
    Description: "Runs JavaScript code"
    Usage: "eval <code>"
    Aliases: []
    Permission:
      - "Zorino#1110"
    AllowedChannels: false
    SlashCommand:
      Enabled: true
      Data:
        Name: eval
        Description: "Runs JavaScript code"
        Options:
          - Type: "String"
            Name: "code"
            Description: "JavaScript code"
            Required: true
```
