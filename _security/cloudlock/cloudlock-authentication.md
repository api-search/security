---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cloudlock Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudLock secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CloudLock
provider_slug: cloudlock
scheme_count: 1
schemes:
- format: Bearer <access_token>
  header: Authorization
  location: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://developer.cisco.com/docs/cloud-security/cloudlock-api-getting-started/
  token_source: 'Cloudlock dashboard: Settings > Authentication & API > Generate access token'
  type: http
slug: cloudlock-authentication
source_filename: cloudlock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.cisco.com/docs/cloud-security/cloudlock-api-getting-started/\ndocs: https://developer.cisco.com/docs/cloud-security/cloudlock-api-getting-started/\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  notes: >-\n    The Cisco Cloudlock API (v2) authenticates every request with a Bearer access\n    token in the Authorization header. Tokens are generated per-tenant from the\n    Cloudlock dashboard under Settings > Authentication & API > Generate. There is\n    no OAuth authorization/token endpoint or scope surface documented for the\n    public API; access is scoped to the tenant the token belongs to. No public\n    OpenAPI is published (the API base host is customer-specific).\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    location: header\n    header: Authorization\n    format: 'Bearer <access_token>'\n    token_source: >-\n      Cloudlock dashboard: Settings > Authentication &\
  \ API > Generate access token\n    sources: [https://developer.cisco.com/docs/cloud-security/cloudlock-api-getting-started/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudlock/refs/heads/main/authentication/cloudlock-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cloud
- Security
- CASB
- Cloud Access Security Broker
- Data Loss Prevention
- Cloud Security
- SaaS Security
- Cisco
---
