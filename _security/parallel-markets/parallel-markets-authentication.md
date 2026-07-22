---
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Parallel Markets Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Parallel Markets secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Parallel Markets
provider_slug: parallel-markets
scheme_count: 2
schemes:
- format: Bearer {apiKey}
  header: Authorization
  location: header
  name: apiKeyBearer
  notes: API keys are created in the Parallel dashboard (app.parallelmarkets.com or demo.parallelmarkets.com) under Settings > Integrations & Exports by admin or controller roles. The full key is shown once at creation; only the Key ID prefix remains visible afterward.
  scheme: bearer
  type: http
  used_by: Server API / Case Management API (v2, current)
- authorizationUrl: https://api.parallelmarkets.com/v1/oauth/authorize
  flow: authorizationCode
  name: oauth2AuthorizationCode
  notes: OAuth2 authorization-code flow (registered client_id/client_secret) used by the v1 Server API and the client-side JavaScript SDK / Passport handoff. HTTPS only; plain HTTP connections are refused.
  scopes:
  - profile
  - accreditation_status
  - identity
  - blockchain
  tokenUrl: https://api.parallelmarkets.com/v1/oauth/token
  type: oauth2
  used_by: v1 legacy OAuth flow + JavaScript SDK Passport authorization
slug: parallel-markets-authentication
source_filename: parallel-markets-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.parallelmarkets.com/docs/server/api-keys\ndocs: https://developer.parallelmarkets.com/docs/server/api-keys\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  location: header\n  header: Authorization\n  format: \"Bearer {apiKey}\"\n  used_by: Server API / Case Management API (v2, current)\n  notes: >-\n    API keys are created in the Parallel dashboard (app.parallelmarkets.com or\n    demo.parallelmarkets.com) under Settings > Integrations & Exports by admin or\n    controller roles. The full key is shown once at creation; only the Key ID\n    prefix remains visible afterward.\n- name: oauth2AuthorizationCode\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://api.parallelmarkets.com/v1/oauth/authorize\n  tokenUrl: https://api.parallelmarkets.com/v1/oauth/token\n  used_by: v1\
  \ legacy OAuth flow + JavaScript SDK Passport authorization\n  scopes: [profile, accreditation_status, identity, blockchain]\n  notes: >-\n    OAuth2 authorization-code flow (registered client_id/client_secret) used by the\n    v1 Server API and the client-side JavaScript SDK / Passport handoff. HTTPS only;\n    plain HTTP connections are refused.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallel-markets/refs/heads/main/authentication/parallel-markets-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Identity
- Identity Verification
- KYC
- AML
- Accreditation
- Compliance
- Financial Services
- Onboarding
- Investor Verification
- Webhooks
---
