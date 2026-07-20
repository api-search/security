---
api_key_in: []
api_specs:
- filename: djamo-webhooks-asyncapi.yml
  format: yaml
  label: Djamo Business API
  slug: djamo-business-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/djamo/refs/heads/main/asyncapi/djamo-webhooks-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Djamo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Djamo secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Djamo
provider_slug: djamo
scheme_count: 2
schemes:
- bearer_prefix: at_
  docs: https://docs.djamo.com/authentication.html
  format: 'Authorization: Bearer <ACCESS_TOKEN>'
  header: Authorization
  location: header
  name: bearerAuth
  scheme: bearer
  type: http
- description: Company identifier required on certain endpoints.
  docs: https://docs.djamo.com/authentication.html
  header: X-company-Id
  in: header
  name: companyIdHeader
  type: apiKey
slug: djamo-authentication
source_filename: djamo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.djamo.com/authentication.html\nsummary:\n  types: [http]\n  http_scheme: bearer\n  token_prefix: at_\n  additional_headers: [X-company-Id]\n  oauth2_flows: []\n  notes: >-\n    Djamo Business API uses a long-lived bearer ACCESS_TOKEN (prefix `at_`) issued\n    to selected partners during onboarding. There is no self-service OAuth flow and\n    no scope surface; access is scoped by the token and business account. Some\n    endpoints additionally require an `X-company-Id` header. All requests must be\n    over HTTPS; plain HTTP is rejected. Token rotation is handled by contacting the\n    Djamo Business account manager. A separate `SECRET_KEY` (issued alongside the\n    access token) is used only to verify webhook HMAC signatures.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearer_prefix: at_\n    location: header\n    header: Authorization\n    format: 'Authorization: Bearer <ACCESS_TOKEN>'\n\
  \    docs: https://docs.djamo.com/authentication.html\n  - name: companyIdHeader\n    type: apiKey\n    in: header\n    header: X-company-Id\n    description: Company identifier required on certain endpoints.\n    docs: https://docs.djamo.com/authentication.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/djamo/refs/heads/main/authentication/djamo-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Financial Services
- Fintech
- Payments
- Banking
- Money Transfer
- Africa
- Côte d'Ivoire
- Sénégal
---
