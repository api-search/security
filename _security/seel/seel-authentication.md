---
api_key_in: []
api_specs:
- filename: seel-openapi.yml
  format: yaml
  label: Seel Commerce Protection API
  slug: seel-commerce-protection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seel/refs/heads/main/openapi/seel-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Seel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seel declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Seel
provider_slug: seel
scheme_count: 1
schemes:
- description: Per-merchant secret API key issued by Seel (request via merchant@seel.com). Sent on every request; must never be exposed in client-side code or public repositories.
  id: SeelApiKey
  in: header
  name: X-Seel-Api-Key
  required: true
  type: apiKey
slug: seel-authentication
source_filename: seel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://developer.seel.com/reference/introduction.md and per-operation\n  reference pages. Seel authenticates every request with a per-merchant API key\n  in the X-Seel-Api-Key header, paired with an X-Seel-Api-Version header to\n  select the API version. No OAuth2/OIDC surface is documented.\nbase_url: https://api-test.seel.com/v1\nschemes:\n  - id: SeelApiKey\n    type: apiKey\n    in: header\n    name: X-Seel-Api-Key\n    description: >-\n      Per-merchant secret API key issued by Seel (request via merchant@seel.com).\n      Sent on every request; must never be exposed in client-side code or public\n      repositories.\n    required: true\nversion_header:\n  name: X-Seel-Api-Version\n  example: 2.6.0\n  description: Selects the API version (e.g. 2.1.0, 2.3.0, 2.6.0).\ntransport:\n  https_required: true\n  notes: All requests must use HTTPS; plain HTTP calls fail.\noauth2: false\nopenid_connect: false\nmutual_tls:\
  \ false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seel/refs/heads/main/authentication/seel-authentication.yml
summary_line: 1 scheme
tags:
- Company
- E-commerce
- Insurance
- Post-Purchase
- Returns
- Extended Warranty
- Fraud
- Payments
---
