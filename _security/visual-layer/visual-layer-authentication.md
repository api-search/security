---
api_key_in: []
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Visual Layer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Visual Layer secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Visual Layer
provider_slug: visual-layer
scheme_count: 3
schemes:
- algorithm: HS256
  applies_to: Visual Layer Cloud API (app.visual-layer.com)
  bearer_format: JWT
  description: JWT bearer token passed in the Authorization header on every request. Tokens are short-lived and self-signed (HS256) client-side from an API key and secret; regenerate periodically.
  header: 'Authorization: Bearer <jwt>'
  name: cloudJwtBearer
  scheme: bearer
  token_claims:
    exp: expiry
    iat: issued-at
    iss: sdk
    kid: api_key
    sub: api_key
  type: http
- credentials_endpoint: https://app.visual-layer.com/api/v1/api_credentials
  description: API key and secret pair used to sign the JWT. Retrieved from the API credentials endpoint (GET /api/v1/api_credentials) while authenticated in the browser session. The secret is shown only once; contact support@visual-layer.com to recover.
  in: cookie/session
  name: apiKeySecret
  type: apiKey
- applies_to: On-premises / self-hosted deployments
  description: On-premises API calls require no authentication; authorization headers are omitted from all requests.
  name: onPremNoAuth
  type: none
slug: visual-layer-authentication
source_filename: visual-layer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.visual-layer.com/api-reference/authentication\ndocs: https://docs.visual-layer.com/api-reference/authentication\nsummary:\n  types: [http, apiKey]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  api_key_provisioning: session-authenticated\n  oauth2_flows: []\n  note: Authentication requirements differ by deployment. The Visual Layer Cloud API requires a\n    short-lived JWT bearer token on every request. On-premises deployments require no authentication and\n    omit the Authorization header entirely.\nschemes:\n- name: cloudJwtBearer\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  applies_to: Visual Layer Cloud API (app.visual-layer.com)\n  description: JWT bearer token passed in the Authorization header on every request. Tokens are\n    short-lived and self-signed (HS256) client-side from an API key and secret; regenerate periodically.\n  header: 'Authorization: Bearer <jwt>'\n  algorithm: HS256\n\
  \  token_claims: {sub: api_key, iat: issued-at, exp: expiry, iss: sdk, kid: api_key}\n- name: apiKeySecret\n  type: apiKey\n  in: cookie/session\n  description: API key and secret pair used to sign the JWT. Retrieved from the API credentials endpoint\n    (GET /api/v1/api_credentials) while authenticated in the browser session. The secret is shown only\n    once; contact support@visual-layer.com to recover.\n  credentials_endpoint: https://app.visual-layer.com/api/v1/api_credentials\n- name: onPremNoAuth\n  type: none\n  applies_to: On-premises / self-hosted deployments\n  description: On-premises API calls require no authentication; authorization headers are omitted from\n    all requests.\nflows:\n  cloud: |\n    1. Log in at https://app.visual-layer.com and call GET /api/v1/api_credentials to obtain api_key + api_secret (secret shown once).\n    2. Sign a short-lived HS256 JWT locally with headers {alg: HS256, typ: JWT, kid: api_key} and payload {sub: api_key, iat, exp, iss: sdk}.\n\
  \    3. Send the JWT as `Authorization: Bearer <jwt>` on every Cloud API request.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visual-layer/refs/heads/main/authentication/visual-layer-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Company
- Computer Vision
- Machine Learning
- Data Management
- Dataset Curation
- Unstructured Data
- Images
- Video
- Semantic Search
- AI
---
