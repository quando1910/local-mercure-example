# Local Mercure Example with Docker
## Introduction
This is the local mercure example with docker. It is enabled the anonymous mode, will allow all the origins, so it's only for development.

## How to run
Just run this:
```
docker-compose up
```

Default Hub information:
- Hub URL: `http://localhost:8081/.well-known/mercure`
- Hub subscriber secret: `MySecret`
- Hub publisher secret: `MySecret`

## Change information
### Change port
- Default is 8081. Navigate to `docker-compose.yml` and replace port 8081. Please make sure not replace `:80`.

### Change the secret
- Default is MySecret. Navigate to `Caddyfile` and update `publisher_jwt` or `subscriber_jwt` to any value you want.
