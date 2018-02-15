# screenhole-web

> Snapshot of Vue screenhole.net frontend prior to React switchover.

## Setup

```
npm install
```

## Development

Serve with hot reload at [localhost:8080](http://localhost:8080). Uses production API by default.

```
npm run dev
```

### Staging API

Run the frontend locally, but read from the staging API.

```
npm run dev:stage
```

### Local API

Run the frontend locally, but read from the local API (e.g. `https://screenhole-api.ngrok.io`, which is part of `heroku local`).

```
npm run dev:local
```

## Build

Build for production with minification. Unlikely you need to do this explicitly, will be run prior to each deploy.

```
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

## Deploy

Deploy an instance of your current working tree (not just what is committed or pushed to GitHub). Will create a new now.sh subdomain, check command output for details.

Uses production API by default.

```
npm run deploy
```

### Staging API

Deploy a new instance, pointing to the staging API.

```
npm run deploy:stage
```

### Local API

Deploy a new instance, pointing to the local API.

```
npm run deploy:local
```

## Promote to Production

To promote a deploy to production, alias a now.sh URL to [screenhole.net](https://screenhole.net).

**Be sure to only promote non-staging/local deploys to production. They will be promoted exactly as-is, their environment will not be modified.**

```
now alias screenhole-web-abcdef.now.sh screenhole.net
```
