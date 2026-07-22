---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Rollee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rollee secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rollee
provider_slug: rollee
scheme_count: 1
schemes:
- bearer_format: JWT
  format: 'Authorization: Bearer <YOUR_TOKEN>'
  header: Authorization
  location: header
  name: bearerAuth
  scheme: bearer
  type: http
slug: rollee-authentication
source_filename: rollee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.getrollee.com/docs/authentication\ndocs: https://developers.getrollee.com/docs/authentication\nsummary:\n  types: [http]\n  scheme: bearer\n  token_format: JWT\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  location: header\n  header: Authorization\n  format: \"Authorization: Bearer <YOUR_TOKEN>\"\ndetails:\n  issuance: >-\n    The initial JWT is provisioned by Rollee (via the contact / onboarding\n    process) with a fixed validity period. Sandbox and production tokens are\n    separate — nothing is shared between the two environments.\n  refresh:\n    production_endpoint: https://api.getrollee.com/api/v0.5/token/refresh\n    sandbox_endpoint: https://api.sand.getrollee.com/api/v0.3/token/refresh\n    method: GET\n    response_example: '{ \"token\": \"YOUR_NEW_TOKEN\" }'\n    note: Generate a new token via the refresh endpoint\
  \ before the current one expires.\n  sessions: >-\n    User- and company-facing flows use short-lived sessions created per user/company;\n    expired sessions are re-established via a session refresh endpoint.\n  errors:\n    unauthorized: 401 returned for invalid/expired tokens\n    success: 200 on valid authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rollee/refs/heads/main/authentication/rollee-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Open Finance
- Income Verification
- Employment Verification
- Payroll Data
- Gig Economy
- Alternative Data
- Underwriting
- Lending
- Fintech
---
