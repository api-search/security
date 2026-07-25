---
api_key_in: []
api_specs:
- filename: appomni-compliance-api-openapi.yml
  format: yaml
  label: AppOmni Compliance API
  slug: appomni-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-compliance-api-openapi.yml
- filename: appomni-policies-api-openapi.yml
  format: yaml
  label: AppOmni Policies API
  slug: appomni-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-policies-api-openapi.yml
- filename: appomni-security-events-api-openapi.yml
  format: yaml
  label: AppOmni Security Events API
  slug: appomni-security-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-security-events-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Appomni Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppOmni secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AppOmni
provider_slug: appomni
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/appomni-openapi.yaml
  type: http
slug: appomni-authentication
source_filename: appomni-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/appomni-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/appomni-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/authentication/appomni-authentication.yml
summary_line: http · 1 scheme
tags:
- SaaS Security
- Compliance
- Threat Detection
- CASB
- Zero Trust
---
