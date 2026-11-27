---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: AcornReply Authentication
name_suffix: Authentication
oauth_flows: []
overview: AcornReply secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AcornReply
provider_slug: acornreply-com
scheme_count: 1
schemes:
- description: Workspace API key (ak_…).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/acornreply-com-openapi.yml
  type: http
slug: acornreply-com-authentication
source_filename: acornreply-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/acornreply-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Workspace API key (ak_…).\n  sources:\n  - openapi/acornreply-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/acornreply-com/authentication/acornreply-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Support
- Software-as-a-Service
- Small Teams
- Artificial Intelligence
- Customer Service
---
