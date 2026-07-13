---
api_key_in: []
api_specs:
- filename: trimble-agriculture-openapi.yml
  format: yaml
  label: Trimble Agriculture Data API
  slug: trimble-agriculture-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trimble-agriculture/refs/heads/main/openapi/trimble-agriculture-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Trimble Agriculture Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trimble Agriculture secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trimble Agriculture
provider_slug: trimble-agriculture
scheme_count: 1
schemes:
- description: OAuth 2.0 bearer token. Register at agdeveloper.trimble.com to obtain API credentials.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/trimble-agriculture-openapi.yml
  type: http
slug: trimble-agriculture-authentication
source_filename: trimble-agriculture-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trimble-agriculture-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token. Register at agdeveloper.trimble.com to obtain API credentials.\n  sources:\n  - openapi/trimble-agriculture-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trimble-agriculture/refs/heads/main/authentication/trimble-agriculture-authentication.yml
summary_line: http · 1 scheme
tags:
- Agriculture
- Farming
- IoT
- Precision Agriculture
- Field Management
- Prescriptions
- Telematics
---
