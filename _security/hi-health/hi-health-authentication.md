---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Hi Health Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Hi Health secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Hi Health
provider_slug: hi-health
scheme_count: 1
schemes:
- environments:
  - api_base: https://partner-api.getpliant.com/api/
    audience: api.getpliant.com/api/integration
    env: production
    token_url: https://infinnityprodinternal.eu.auth0.com/oauth/token
  - api_base: https://sandbox.partner-api.getpliant.com/api/
    audience: api.staging.infinnitytest.com/api/integration
    env: sandbox
    token_url: https://infinnitystaginginternal.eu.auth0.com/oauth/token
  flow: clientCredentials
  name: OAuth2ClientCredentials
  provider: Auth0
  quota:
    exceeded_status: 429
    headers:
    - Auth0-Client-Quota-Limit
  token_transport: Bearer token in Authorization header
  token_ttl_seconds: 86400
  type: oauth2
slug: hi-health-authentication
source_filename: hi-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://customer-api.getpliant.com/docs/authenticated-api-usage\nnote: >-\n  Derived from the Pliant Pro API (Customer) authentication docs — the API powering hi.health by\n  Pliant. No public OpenAPI is downloadable from the ReadMe-hosted portal, so this profile is\n  captured from the published auth documentation rather than a machine-derived securityScheme.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_transport: bearer\n  backend_only: true\n  https_required: true\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  provider: Auth0\n  token_transport: Bearer token in Authorization header\n  token_ttl_seconds: 86400\n  environments:\n  - env: production\n    token_url: https://infinnityprodinternal.eu.auth0.com/oauth/token\n    audience: api.getpliant.com/api/integration\n    api_base: https://partner-api.getpliant.com/api/\n  - env: sandbox\n    token_url:\
  \ https://infinnitystaginginternal.eu.auth0.com/oauth/token\n    audience: api.staging.infinnitytest.com/api/integration\n    api_base: https://sandbox.partner-api.getpliant.com/api/\n  quota:\n    headers: [Auth0-Client-Quota-Limit]\n    exceeded_status: 429\nnotes:\n- The authorization flow must be handled exclusively by a secure backend.\n- All communication requires HTTPS; plain HTTP is unsupported.\n- PCI-DSS certified sensitive-card-data endpoints use a dedicated host pci-api.getpliant.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hi-health/refs/heads/main/authentication/hi-health-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Health
- Insurance
- Payments
- Fintech
- Card Issuing
- Reimbursement
- InsurTech
- Digital Health
- Speedinvest
---
