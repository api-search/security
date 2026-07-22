---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Plextrac Llc Authentication
name_suffix: Authentication
oauth_flows: []
overview: PlexTrac, LLC secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PlexTrac, LLC
provider_slug: plextrac-llc
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: PlexTrac uses a JWT bearer token. Obtain the token by POSTing credentials to /api/v1/authenticate against your PlexTrac instance; the returned JWT is sent on subsequent requests in the Authorization header as "Bearer <token>". Tokens expire after 15 minutes and are renewed with the refresh-token endpoint. Accounts with multi-factor authentication enabled receive a code on the initial authenticate call and complete a follow-up MFA request before a token is issued.
  name: bearerAuth
  scheme: bearer
  sources:
  - docs.plextrac.com
  type: http
slug: plextrac-llc-authentication
source_filename: plextrac-llc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.plextrac.com/\ndocs: https://docs.plextrac.com/\nsummary:\n  types:\n  - http\n  http_scheme: bearer\n  bearer_format: JWT\n  token_endpoint: /api/v1/authenticate\n  token_lifetime_minutes: 15\n  mfa_supported: true\n  refresh_supported: true\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    PlexTrac uses a JWT bearer token. Obtain the token by POSTing credentials to\n    /api/v1/authenticate against your PlexTrac instance; the returned JWT is sent\n    on subsequent requests in the Authorization header as \"Bearer <token>\". Tokens\n    expire after 15 minutes and are renewed with the refresh-token endpoint.\n    Accounts with multi-factor authentication enabled receive a code on the initial\n    authenticate call and complete a follow-up MFA request before a token is issued.\n  sources:\n  - docs.plextrac.com\nflows:\n  password_style:\n    authenticate:\
  \ POST /api/v1/authenticate\n    mfa: POST /api/v1/authenticate/mfa\n    refresh: PUT /api/v1/token\nnotes:\n- The API base URL is the customer's own PlexTrac instance host (the SaaS instance\n  is app.plextrac.com); self-hosted/dedicated deployments use their own host.\n- Authentication requests are rate limited to 10 per minute.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plextrac-llc/refs/heads/main/authentication/plextrac-llc-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cybersecurity
- Penetration Testing
- Vulnerability Management
- Security Reporting
- Exposure Management
- Offensive Security
- MSSP
- Remediation
---
