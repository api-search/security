---
api_key_in: []
api_specs:
- filename: jurisign-api-openapi.yml
  format: yaml
  label: JuriSign API
  slug: jurisign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jurisign Authentication
name_suffix: Authentication
oauth_flows: []
overview: JuriSign secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JuriSign
provider_slug: jurisign
scheme_count: 1
schemes:
- description: 'Obtain a token via POST /auth/token, then pass it as: Authorization: Bearer {token}'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/jurisign-api-openapi.yml
  type: http
slug: jurisign-authentication
source_filename: jurisign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-31'\nmethod: derived\nsource: openapi/jurisign-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Obtain a token via POST /auth/token, then pass it as: Authorization: Bearer\n    {token}'\n  sources:\n  - openapi/jurisign-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/authentication/jurisign-authentication.yml
summary_line: http · 1 scheme
tags:
- Electronic Signature
- E-Signature
- eIDAS
- Document Signing
- PDF
- Webhook
- OTP
- GDPR
- France
- Legal Tech
- Identity Verification
- Audit Trail
- data-residency-eu
---
