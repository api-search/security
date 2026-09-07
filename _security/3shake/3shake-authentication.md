---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 3shake-reckoner-external-api-openapi.yml
  format: yaml
  label: Reckoner External API
  slug: reckoner-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3shake/refs/heads/main/openapi/3shake-reckoner-external-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: 3Shake Authentication
name_suffix: Authentication
oauth_flows: []
overview: 3-shake secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 3-shake
provider_slug: 3shake
scheme_count: 2
schemes:
- applies_to: default security requirement for all 14 business operations
  bearerFormat: Access token
  description: アクセストークン（pat_ プレフィックス） — access token, pat_ prefix
  name: BearerAccessAuth
  scheme: bearer
  sources:
  - openapi/3shake-reckoner-external-api-openapi.yml
  type: http
- applies_to: operation-level override on POST /auth/token/refresh (authTokenRefresh) only
  bearerFormat: Refresh token
  description: リフレッシュトークン（prt_ プレフィックス） — refresh token, prt_ prefix
  name: BearerRefreshAuth
  scheme: bearer
  sources:
  - openapi/3shake-reckoner-external-api-openapi.yml
  type: http
slug: 3shake-authentication
source_filename: 3shake-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/3shake-reckoner-external-api-openapi.yml\ndocs: https://developers.reckoner-api.com/reckoner-external-api.html\nnote: >-\n  Upgraded from the mechanical derive, which deduplicated the two bearer schemes into one. Both are declared in the\n  contract and they are NOT interchangeable — the access token authorises every business operation, the refresh token\n  authorises only POST /auth/token/refresh. Token prefixes (pat_ / prt_) are quoted from the schemes' own descriptions.\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\n  token_prefixes: ['pat_', 'prt_']\nschemes:\n- name: BearerAccessAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Access token\n  description: アクセストークン（pat_ プレフィックス） — access token, pat_ prefix\n  applies_to: default security requirement for all 14 business operations\n  sources: [openapi/3shake-reckoner-external-api-openapi.yml]\n- name: BearerRefreshAuth\n\
  \  type: http\n  scheme: bearer\n  bearerFormat: Refresh token\n  description: リフレッシュトークン（prt_ プレフィックス） — refresh token, prt_ prefix\n  applies_to: operation-level override on POST /auth/token/refresh (authTokenRefresh) only\n  sources: [openapi/3shake-reckoner-external-api-openapi.yml]\ntoken_lifecycle:\n  refresh_operation: authTokenRefresh\n  refresh_path: POST /auth/token/refresh\n  refresh_transport: refresh token presented in the Authorization header\n  response_fields: [access_token, expires_at]\n  expires_at_format: RFC 3339 date-time\n  revocation_signals:\n    observed_in_contract: [TOKEN_INVALID, TOKEN_EXPIRED, TOKEN_REVOKED]\n    http_status: 401\nother_apis:\n- api: Securify Scan Public API\n  scheme: public API token created in the Securify console and sent on the request\n  docs: https://help-scan.securify.jp/hc/ja/articles/25133482168345\n  method: searched\n  evidence:\n  - url: https://www.securify.jp/news/securify-update-api/\n    status: 200\n    note: >-\n      The\
  \ provider's own release note describes creating and deleting API tokens in the console and calling the API to\n      start a diagnosis, returning a diagnosis ID. The step-by-step reference is a Zendesk help centre behind a\n      Cloudflare bot challenge (HTTP 403 to this crawler), so the exact header name could not be read first-hand and is\n      deliberately NOT recorded here rather than guessed.\n  - url: https://scan.securify.jp/api/v1\n    status: 401\n    note: 'unauthenticated GET returns {\"title\":\"Unauthenticated\",\"status\":401,\"detail\":\"無効なリクエストです。\"}'\nlegacy:\n- api: Reckoner CDP (legacy streaming/query surface)\n  scheme: custom HMAC-SHA256 request signing\n  header: 'Authorization: RECKONER-CDP <AccessKeyID>:<base64(HMAC-SHA256(SecretAccessKey, METHOD\\nContent-MD5\\nContent-Type\\nDate))>'\n  credentials: Access Key ID + Secret Access Key, issued from the Management page of the Reckoner web UI\n  source: https://raw.githubusercontent.com/3-shake/reckoner-cdp-go/master/client.go\n\
  \  method: searched\n  note: Read from the provider's own published client library. Superseded by the pat_/prt_ bearer model above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3shake/refs/heads/main/authentication/3shake-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- SRE
- Data Integration
- ETL
- iPaaS
- Workflow Automation
- Vulnerability Scanning
- Attack Surface Management
- Cloud Security
- DevSecOps
- SBOM
- Kubernetes
- Japan
---
