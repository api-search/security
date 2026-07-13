---
api_key_in: []
api_specs:
- filename: didomi-platform-api-openapi.yml
  format: yaml
  label: Didomi Platform API
  slug: didomi-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didomi/refs/heads/main/openapi/didomi-platform-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Didomi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Didomi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Didomi
provider_slug: didomi
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/didomi-platform-api-openapi.yml
  type: http
slug: didomi-authentication
source_filename: didomi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/didomi-platform-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/didomi-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/didomi/refs/heads/main/authentication/didomi-authentication.yml
summary_line: http · 1 scheme
tags:
- Advertising
- AdTech
- CCPA
- CMP
- Consent
- Consent Management
- DSAR
- Data Privacy
- GDPR
- IAB TCF
- MarTech
- Preference Management
- Privacy
- Privacy Requests
- Regulatory Compliance
---
