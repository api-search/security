---
api_key_in: []
api_specs:
- filename: ketryx-build-api-openapi.yml
  format: yaml
  label: Ketryx Build API
  slug: ketryx-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ketryx/refs/heads/main/openapi/ketryx-build-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ketryx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ketryx secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ketryx
provider_slug: ketryx
scheme_count: 1
schemes:
- description: 'A Ketryx API key passed as an HTTP Bearer token in the Authorization header ("Authorization: Bearer <api-key>"). API keys are issued per project in the Ketryx application.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ketryx-build-api-openapi.yml
  type: http
slug: ketryx-authentication
source_filename: ketryx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/ketryx-build-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'A Ketryx API key passed as an HTTP Bearer token in the Authorization header\n    (\"Authorization: Bearer <api-key>\"). API keys are issued per project in the Ketryx application.'\n  sources:\n  - openapi/ketryx-build-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ketryx/refs/heads/main/authentication/ketryx-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Medical Devices
- Life Sciences
- Compliance
- Regulatory
- Application Lifecycle Management
- Quality Management
- SBOM
- DevOps
- Healthcare
- Governance
- CI/CD
---
