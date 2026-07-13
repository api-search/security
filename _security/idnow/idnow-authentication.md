---
api_key_in:
- header
api_specs:
- filename: idnow-openapi.yml
  format: yaml
  label: IDnow Identifications API
  slug: idnow-identifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idnow/refs/heads/main/openapi/idnow-openapi.yml
- filename: idnow-openapi.yml
  format: yaml
  label: IDnow Results & Retrieval API
  slug: idnow-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idnow/refs/heads/main/openapi/idnow-openapi.yml
- filename: idnow-openapi.yml
  format: yaml
  label: IDnow AutoIdent API
  slug: idnow-autoident-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idnow/refs/heads/main/openapi/idnow-openapi.yml
- filename: idnow-openapi.yml
  format: yaml
  label: IDnow VideoIdent API
  slug: idnow-videoident-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idnow/refs/heads/main/openapi/idnow-openapi.yml
- filename: idnow-openapi.yml
  format: yaml
  label: IDnow Webhooks
  slug: idnow-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idnow/refs/heads/main/openapi/idnow-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Idnow Authentication
name_suffix: Authentication
oauth_flows: []
overview: IDnow secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IDnow
provider_slug: idnow
scheme_count: 1
schemes:
- description: JWT returned by the login endpoint, sent on every authenticated request.
  in: header
  name: LoginToken
  parameter: X-API-LOGIN-TOKEN
  sources:
  - openapi/idnow-openapi.yml
  type: apiKey
slug: idnow-authentication
source_filename: idnow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/idnow-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: LoginToken\n  type: apiKey\n  in: header\n  parameter: X-API-LOGIN-TOKEN\n  description: JWT returned by the login endpoint, sent on every authenticated request.\n  sources:\n  - openapi/idnow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idnow/refs/heads/main/authentication/idnow-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Identity Verification
- KYC
- Identity Proofing
- AML
- eSign
---
