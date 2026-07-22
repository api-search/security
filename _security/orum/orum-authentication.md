---
api_key_in: []
api_specs:
- filename: orum-openapi-original.yml
  format: yaml
  label: Orum API
  slug: orum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/openapi/orum-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Orum Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Orum secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Orum
provider_slug: orum
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 29
    tokenUrl: https://api-sandbox.orum.io/oauth/token
  name: oauth2
  sources:
  - openapi/orum-openapi-original.yml
  type: oauth2
slug: orum-authentication
source_filename: orum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/orum-openapi-original.yml\ndocs: https://docs.orum.io/guides/api-authentication\nnotes: >-\n  OAuth 2.0 client-credentials. Create client_id/client_secret in Monitor\n  (Developer Tools -> API Authentication); max two credential sets per Enterprise\n  per environment. Exchange at /oauth/token for a bearer access token; the secret\n  is shown only once. Rotate by generating a new set before deleting the old.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-sandbox.orum.io/oauth/token\n    scopes: 29\n  sources:\n  - openapi/orum-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orum/refs/heads/main/authentication/orum-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Payments
- Fintech
- Banking
- Instant Payments
- ACH
- Money Movement
- Bank Account Verification
---
