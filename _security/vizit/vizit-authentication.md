---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Vizit Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Vizit secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Vizit
provider_slug: vizit
scheme_count: 2
schemes:
- audience: https://ext.vizit.com
  audience_note: The audience value is constant across production and every dev environment.
  flow: clientCredentials
  identity_provider: Auth0
  name: OAuth2ClientCredentials
  operation: createToken
  required_parameters:
  - description: Machine-to-machine client ID issued by Vizit.
    name: client_id
  - description: Machine-to-machine client secret issued by Vizit.
    name: client_secret
  - description: Always https://ext.vizit.com.
    name: audience
  - description: Auth0 organization ID issued by Vizit during onboarding. Required because the Auth0 client grant uses organization_usage; require.
    name: organization
  - description: Must be client_credentials.
    name: grant_type
  scopes: []
  scopes_documented: false
  sources:
  - https://docs.vizit.com/standards/authentication
  - https://docs.vizit.com/api/authentication/createToken
  token_url: https://ext.vizit.com/auth/token
  type: oauth2
- applies_to: All protected /v1/** endpoints
  bearerFormat: JWT
  header: 'Authorization: Bearer <access_token>'
  name: BearerAuth
  scheme: bearer
  sources:
  - https://docs.vizit.com/standards/authentication
  type: http
slug: vizit-authentication
source_filename: vizit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://docs.vizit.com/standards/authentication\ndocs: https://docs.vizit.com/standards/authentication\nnotes: 'Derived from the provider''s published Authentication standard page and the\n  createToken operation reference. No downloadable OpenAPI document is served, so the\n  securityScheme shapes below are transcribed from the published docs rather than\n  parsed from a spec file.'\nsummary:\n  types:\n  - oauth2\n  - http\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  model: machine-to-machine (server-to-server) only\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://ext.vizit.com/auth/token\n  operation: createToken\n  identity_provider: Auth0\n  scopes: []\n  scopes_documented: false\n  audience: https://ext.vizit.com\n  audience_note: The audience value is constant across production and every dev environment.\n  required_parameters:\n  - name: client_id\n\
  \    description: Machine-to-machine client ID issued by Vizit.\n  - name: client_secret\n    description: Machine-to-machine client secret issued by Vizit.\n  - name: audience\n    description: Always https://ext.vizit.com.\n  - name: organization\n    description: Auth0 organization ID issued by Vizit during onboarding. Required because\n      the Auth0 client grant uses organization_usage; require.\n  - name: grant_type\n    description: Must be client_credentials.\n  sources:\n  - https://docs.vizit.com/standards/authentication\n  - https://docs.vizit.com/api/authentication/createToken\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: All protected /v1/** endpoints\n  header: 'Authorization: Bearer <access_token>'\n  sources:\n  - https://docs.vizit.com/standards/authentication\ntoken:\n  lifetime_seconds: 86400\n  lifetime_note: Returned as expires_in on the token response; documented example is 86400\n    seconds (24 hours).\n  caching_guidance:\
  \ Cache the token until it expires rather than requesting one per API call.\n  refresh_guidance: On a 401, request a fresh token and retry once.\n  unauthenticated_endpoints:\n  - POST /auth/token\ncredentials:\n  issuance: Provisioned by Vizit per organization and per environment during onboarding.\n  self_service: false\n  environment_scoped: true\n  environment_note: Production credentials work only against production; dev1 credentials\n    only against dev1.\n  handling_guidance:\n  - Store client_secret only in secure server-side systems or a secrets manager.\n  - Do not embed machine-to-machine credentials in browser apps, mobile apps, or any\n    distributed client.\n  - Treat client_secret as a long-lived secret and the access token as a short-lived credential.\nx-evidence:\n  fetched: '2026-08-02'\n  urls:\n  - url: https://docs.vizit.com/standards/authentication\n    http_status: 200\n  - url: https://docs.vizit.com/llms-full.txt\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vizit/refs/heads/main/authentication/vizit-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Visual AI
- Ecommerce
- Digital Shelf
- Image Analytics
- Content Effectiveness
- Retail Media
- Product Detail Pages
- Machine Learning
- Generative AI
---
