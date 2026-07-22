---
api_key_in: []
api_specs:
- filename: soveren-object-api-openapi.yml
  format: yaml
  label: Soveren Object API
  slug: soveren-object-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soveren/refs/heads/main/openapi/soveren-object-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Soveren Authentication
name_suffix: Authentication
oauth_flows: []
overview: Soveren secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Soveren
provider_slug: soveren
scheme_count: 1
schemes:
- description: Bearer token generated in the Soveren app under Integrations - External API.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/soveren-object-api-openapi.yml
  type: http
slug: soveren-authentication
source_filename: soveren-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/soveren-object-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token generated in the Soveren app under Integrations - External API.\n  sources:\n  - openapi/soveren-object-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soveren/refs/heads/main/authentication/soveren-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Infra Devtools
- Data Security
- DSPM
- DDR
- Data Privacy
- Kubernetes
- Compliance
- Security
---
