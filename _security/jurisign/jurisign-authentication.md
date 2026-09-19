---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jurisign-account-api-openapi.yml
  format: yaml
  label: JuriSign Account API
  slug: jurisign-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-account-api-openapi.yml
- filename: jurisign-authentication-api-openapi.yml
  format: yaml
  label: JuriSign Authentication API
  slug: jurisign-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-authentication-api-openapi.yml
- filename: jurisign-bulk-api-openapi.yml
  format: yaml
  label: JuriSign Bulk API
  slug: jurisign-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-bulk-api-openapi.yml
- filename: jurisign-documents-api-openapi.yml
  format: yaml
  label: JuriSign Documents API
  slug: jurisign-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-documents-api-openapi.yml
- filename: jurisign-public-forms-api-openapi.yml
  format: yaml
  label: JuriSign Public Forms API
  slug: jurisign-public-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-public-forms-api-openapi.yml
- filename: jurisign-sign-requests-api-openapi.yml
  format: yaml
  label: JuriSign Sign Requests API
  slug: jurisign-sign-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-sign-requests-api-openapi.yml
- filename: jurisign-templates-api-openapi.yml
  format: yaml
  label: JuriSign Templates API
  slug: jurisign-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-templates-api-openapi.yml
- filename: jurisign-webhooks-api-openapi.yml
  format: yaml
  label: JuriSign Webhooks API
  slug: jurisign-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
