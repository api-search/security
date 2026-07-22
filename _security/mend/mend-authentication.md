---
api_key_in: []
api_specs:
- filename: mend-platform-openapi-original.json
  format: json
  label: Mend AppSec Platform API
  slug: mend-appsec-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mend/refs/heads/main/openapi/mend-platform-openapi-original.json
- filename: mend-sca-openapi-original.json
  format: json
  label: Mend SCA API
  slug: mend-sca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mend/refs/heads/main/openapi/mend-sca-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mend Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mend secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mend
provider_slug: mend
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token Bearer
  name: bearer-key
  scheme: bearer
  sources:
  - openapi/mend-platform-openapi-original.json
  - openapi/mend-sca-openapi-original.json
  type: http
slug: mend-authentication
source_filename: mend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mend-platform-openapi-original.json, openapi/mend-sca-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer-key\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token Bearer\n  sources:\n  - openapi/mend-platform-openapi-original.json\n  - openapi/mend-sca-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mend/refs/heads/main/authentication/mend-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Security
- Software Composition Analysis
- SAST
- Container Security
- AI Security
- Dependency Management
- Vulnerability Management
- DevSecOps
- SBOM
- Open Source Security
- Company
---
