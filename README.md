# Free Fire Player Info API (OB55 Premium)

High-performance Free Fire Player Lookup REST API built with Python Flask, Protobuf, and Vercel Serverless support.

## 🚀 Endpoints

### 1. Player Information
```http
GET /info?uid=<PLAYER_UID>
```

#### Example Request:
```bash
curl "https://<your-vercel-domain>/info?uid=7390429920"
```

#### Response Structure:
```json
{
  "status": "success",
  "server_used": "IND",
  "BasicInformation": {
    "Name": "PlayerNickname",
    "UID": "7390429920",
    "Level": 65,
    "Region": "IND",
    "Likes": 12500
  },
  "GuildInformation": {
    "GuildName": "Team Name",
    "GuildID": "12345678"
  }
}
```

### 2. API Status & Token Check
```http
GET /status
```

## 🛠️ Deploy on Vercel

1. Import this repository in [Vercel](https://vercel.com/new).
2. Framework Preset: **Other**.
3. Deploy!