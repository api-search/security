---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Hihealth Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: hi.health secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: hi.health
provider_slug: hihealth
scheme_count: 1
schemes:
- audience:
    production: api.getpliant.com/api/integration
    sandbox: api.staging.infinnitytest.com/api/integration
  constraint: The authorization flow must be handled exclusively by a secure backend; web frontends and mobile apps must not call the API directly or expose credentials.
  credentials: client_id + client_secret (issued during partner onboarding)
  flow: clientCredentials
  grant_type: client_credentials
  identity_provider: Auth0
  name: OAuth2ClientCredentials
  token_header: 'Authorization: Bearer <token>'
  token_ttl_seconds: 86400
  token_type: Bearer
  token_urls:
    production: https://infinnityprodinternal.eu.auth0.com/oauth/token
    sandbox: https://infinnitystaginginternal.eu.auth0.com/oauth/token
  type: oauth2
slug: hihealth-authentication
source_filename: hihealth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://partner.getpliant.com/docs/authenticated-api-usage.md\ndocs: https://partner.getpliant.com/docs/authenticated-api-usage.md\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  identity_provider: Auth0\n  token_urls:\n    production: https://infinnityprodinternal.eu.auth0.com/oauth/token\n    sandbox: https://infinnitystaginginternal.eu.auth0.com/oauth/token\n  audience:\n    production: api.getpliant.com/api/integration\n    sandbox: api.staging.infinnitytest.com/api/integration\n  grant_type: client_credentials\n  credentials: client_id + client_secret (issued during partner onboarding)\n  token_type: Bearer\n  token_ttl_seconds: 86400\n  token_header: 'Authorization: Bearer <token>'\n  constraint: >-\n    The authorization flow must be handled exclusively by a secure backend;\n    web frontends\
  \ and mobile apps must not call the API directly or expose\n    credentials.\nnotes: >-\n  Bearer tokens are valid until their TTL (24h) is reached and are not\n  invalidated earlier. Fetch a new token shortly before expiry. Scope/permission\n  model is documented separately (see scopes/hihealth-scopes.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hihealth/refs/heads/main/authentication/hihealth-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Insurance
- Payments
- Cards
- Fintech
- Health
- Cards-as-a-Service
- Embedded Finance
- Reimbursement
- Claims
---
