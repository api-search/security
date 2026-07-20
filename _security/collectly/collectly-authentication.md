---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Collectly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Collectly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Collectly
provider_slug: collectly
scheme_count: 1
schemes:
- bearer_format: JWT
  credentials:
  - format: hex string (no hyphens)
    name: COMPANY_ID
  - format: hex string (no hyphens)
    name: COMPANY_SECRET
  description: 'Collectly''s Partners API requires a JSON Web Token (JWT) on every request. The partner mints the token from two credentials issued by Collectly: COMPANY_ID and COMPANY_SECRET (hex strings without hyphens). The signed token is sent in the Authorization header on every request.'
  header: Authorization
  location: header
  name: partnerJWT
  notes:
  - A separate patient JWT can be minted to log a patient into the hosted patient portal / embedded pages (see conventions + components artifacts).
  scheme: bearer
  sources:
  - docs.collectly.co
  type: http
slug: collectly-authentication
source_filename: collectly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.collectly.co/\ndocs: https://docs.collectly.co/\nsummary:\n  types: [http]\n  scheme: bearer\n  bearer_format: JWT\n  oauth2_flows: []\n  api_key_in: []\nschemes:\n  - name: partnerJWT\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    description: >-\n      Collectly's Partners API requires a JSON Web Token (JWT) on every request.\n      The partner mints the token from two credentials issued by Collectly:\n      COMPANY_ID and COMPANY_SECRET (hex strings without hyphens). The signed\n      token is sent in the Authorization header on every request.\n    location: header\n    header: Authorization\n    credentials:\n      - name: COMPANY_ID\n        format: hex string (no hyphens)\n      - name: COMPANY_SECRET\n        format: hex string (no hyphens)\n    notes:\n      - A separate patient JWT can be minted to log a patient into the hosted\n        patient portal / embedded pages (see conventions\
  \ + components artifacts).\n    sources: [docs.collectly.co]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collectly/refs/heads/main/authentication/collectly-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthtech
- Revenue Cycle Management
- Patient Payments
- Medical Billing
- Payments
- Healthcare
- Insurance Eligibility
---
