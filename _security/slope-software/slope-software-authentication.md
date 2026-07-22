---
api_key_in: []
api_specs:
- filename: slope-software-openapi-original.json
  format: json
  label: Slope API
  slug: slope-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slope-software/refs/heads/main/openapi/slope-software-openapi-original.json
auth_types:
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Slope Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Slope Software secures its APIs with http-bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Slope Software
provider_slug: slope-software
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JWT bearer access token. Exchange API credentials at POST /api/v1/Authorize to receive an ApiTokenDto, send it as `Authorization: Bearer <token>` on every call, and renew it via POST /api/v1/Authorize/Refresh. Documented in the SLOPE API overview (slopesoftware.com/wp-content/uploads/2022/02/SLOPE-API.pdf).'
  name: API Token
  scheme: bearer
  sources:
  - openapi/slope-software-openapi-original.json
  type: http
slug: slope-software-authentication
source_filename: slope-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/slope-software-openapi-original.json\ndocs: https://api.slopesoftware.com/\nsummary:\n  types:\n  - http-bearer\n  bearer_format: JWT\n  token_endpoint: /api/v1/Authorize\n  refresh_endpoint: /api/v1/Authorize/Refresh\n  console_sso: OpenID Connect via Frontegg (auth.slopesoftware.com)\nschemes:\n- name: API Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT bearer access token. Exchange API credentials at POST /api/v1/Authorize to receive\n    an ApiTokenDto, send it as `Authorization: Bearer <token>` on every call, and renew it via POST /api/v1/Authorize/Refresh.\n    Documented in the SLOPE API overview (slopesoftware.com/wp-content/uploads/2022/02/SLOPE-API.pdf).'\n  sources:\n  - openapi/slope-software-openapi-original.json\nplatform_auth:\n  name: Frontegg OpenID Connect\n  type: openIdConnect\n  issuer: https://auth.slopesoftware.com\n  discovery: https://auth.slopesoftware.com/.well-known/openid-configuration\n\
  \  grant_types:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:device_code\n  scopes:\n  - openid\n  - profile\n  - email\n  note: Console/SSO login for the SLOPE web application (app.slopesoftware.com); distinct from the API\n    Token used by the REST API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slope-software/refs/heads/main/authentication/slope-software-authentication.yml
summary_line: http-bearer · 1 scheme
tags:
- Company
- Actuarial
- Insurance
- Actuarial Modeling
- Valuation
- Financial Services
- Life Insurance
- Annuities
- Pension
- Risk Management
- Cloud
- Reporting
---
