---
api_key_in: []
api_specs:
- filename: dome9-api
  format: yaml
  label: Dome9 API
  slug: dome9-api
  spec_type: Postman
  url: https://www.postman.com/dome9-security/workspace/dome9-api
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dome9 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dome9 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dome9
provider_slug: dome9
scheme_count: 1
schemes:
- description: HTTP Basic with username = API key id and password = API key secret.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/dome9-openapi.yml
  type: http
slug: dome9-authentication
source_filename: dome9-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dome9-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with username = API key id and password = API key secret.\n  sources:\n  - openapi/dome9-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dome9/refs/heads/main/authentication/dome9-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Security
- Compliance
- Infrastructure Security
- Multi-Cloud
- Security Posture Management
---
