# Cogoland REST API (reverse engineered)

Unofficial API reference and small CLI for the Cogoland mobile app
(`com.nfcogos.map`). This repository is archived and read-only.

## What is included

- `openapi.json`: OpenAPI 3.0 document for the API.
- `cogoland`: Python CLI that calls the documented endpoints.
- `docs/endpoints.md`: Endpoint notes grouped by domain.

## Base URL

```text
https://api.nfcogos.com
```

WebSocket transport uses Socket.IO on the same base URL.

## Authentication

The mobile client sends a bearer token:

```text
Authorization: Bearer <token>
```

The token comes from the Google/Apple sign-in flow and is exchanged through
`/auth/token` or `/auth/google`.

## Quick start

```bash
# Store a token locally. Use your own token value.
export COGOLAND_TOKEN="<your-token>"

# Call an endpoint
./cogoland request GET /profile

# Search users
./cogoland request GET '/users?search=test'
```

## CLI commands

```text
cogoland token set <token>      Store a bearer token in ~/.config/cogoland/token
cogoland token show             Show whether a token is configured
cogoland request METHOD PATH    Call any documented endpoint
```

Example:

```bash
./cogoland token set eyJ...
./cogoland request GET /v2/feed?limit=15
./cogoland request POST /posts --data '{"content":"hello"}'
```

## Security

This project stores tokens only in the user profile under
`~/.config/cogoland/token`. Do not commit real tokens. Examples use synthetic
data.

## Disclaimer

This repository is not affiliated with Cogoland or NFCogos. Endpoints and
request or response bodies were inferred from the mobile application. The
API may change without notice.
