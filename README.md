# Netomi Webhook Inspector

A local proxy server + UI to inspect custom attributes from Netomi's webhook history API — no CORS issues.

## Setup

### 1. Install dependencies
```bash
npm install
```

### 2. Start the server
```bash
node server.js
```

### 3. Open the UI
Visit: **http://localhost:3000**

---

## How it works

```
Browser → localhost:3000/proxy/webhook-history → chatapps-us.netomi.com
```

The browser talks to the local Express server (no CORS), and the server forwards the request to Netomi.

## Files
- `server.js` — Express proxy server
- `public/index.html` — The UI
