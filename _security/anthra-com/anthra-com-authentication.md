---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Anthra Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anthra declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Anthra
provider_slug: anthra-com
scheme_count: 3
schemes:
- description: 'Use the standard HTTP Authorization header: Authorization: Bearer <token>. Tokens start with prefix `ant_live_` and are ~50 characters of URL-safe base64.'
  scheme: bearer
  type: http
- description: Fallback header for clients that cannot set Authorization. Send the raw token. If both Authorization and X-API-Key are present, Authorization wins.
  in: header
  name: X-API-Key
  type: apiKey
- description: 'Cookie-session fallback: if a request to /api/v1/* arrives without a bearer token but carries an authenticated Auth.js session cookie, the caller is treated as the signed‑in user with all scopes. Production should use Bearer token.'
  name: authjs.session
  type: cookie
slug: anthra-com-authentication
source_filename: anthra-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://anthra.com/docs/authentication\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"Use the standard HTTP Authorization header: Authorization: Bearer <token>. Tokens start with prefix `ant_live_` and are ~50 characters of URL-safe base64.\"\n  - type: apiKey\n    in: header\n    name: X-API-Key\n    description: \"Fallback header for clients that cannot set Authorization. Send the raw token. If both Authorization and X-API-Key are present, Authorization wins.\"\n  - type: cookie\n    name: authjs.session\n    description: \"Cookie-session fallback: if a request to /api/v1/* arrives without a bearer token but carries an authenticated Auth.js session cookie, the caller is treated as the signed‑in user with all scopes. Production should use Bearer token.\"\nscopes:\n  - name: books:read\n    description: \"Read books and chapters.\"\n  - name: books:write\n    description: \"Create, update, delete, and outline\
  \ books and chapters.\"\n  - name: generation:run\n    description: \"Run the AI generation pipeline – outline, write, rewrite, narrate.\"\n  - name: publish:write\n    description: \"Publish or unpublish books and change reader visibility.\"\n  - name: account:read\n    description: \"Read account profile and token usage.\"\n  - name: analytics:read\n    description: \"Read per‑chapter reader analytics for published books.\"\n"
source_yaml_url: https://artifacts.apis.io/anthra-com/authentication/anthra-com-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- BookCreation
- Writing
- Illustration
- Audiobook
---
