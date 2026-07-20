---
api_key_in:
- header
api_specs:
- filename: class-fka-classedu-openapi.yml
  format: yaml
  label: Class Developer API
  slug: class-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/class-fka-classedu/refs/heads/main/openapi/class-fka-classedu-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Class Fka Classedu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Class (fka ClassEDU) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Class (fka ClassEDU)
provider_slug: class-fka-classedu
scheme_count: 1
schemes:
- description: Per-organization API key presented as a Bearer token in the Authorization header. The key secret is displayed only once, at key creation, in the Class Admin UI API Keys page (which is also where the organization's unique base URL is shown). Each key is granted a set of permission scopes; selecting a write scope automatically grants the matching read scope.
  format: 'Authorization: Bearer <api_key_secret>'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/class-fka-classedu-openapi.yml
  type: http
slug: class-fka-classedu-authentication
source_filename: class-fka-classedu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/class-fka-classedu-openapi.yml\ndocs: https://developer.class.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  model: api-key-bearer-with-scopes\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <api_key_secret>'\n  description: >-\n    Per-organization API key presented as a Bearer token in the Authorization\n    header. The key secret is displayed only once, at key creation, in the Class\n    Admin UI API Keys page (which is also where the organization's unique base\n    URL is shown). Each key is granted a set of permission scopes; selecting a\n    write scope automatically grants the matching read scope.\n  sources:\n  - openapi/class-fka-classedu-openapi.yml\nscopes:\n- scope: class:read\n  description: Read class information.\n- scope: class:write\n  description: Create, update and remove classes (implies class:read).\n\
  - scope: enrollment:read\n  description: Read enrollment information and launch links.\n- scope: enrollment:write\n  description: Create, update and remove enrollments (implies enrollment:read).\n- scope: attendance:read\n  description: Read attendance reporting.\n- scope: metrics:read\n  description: Read engagement metrics reporting.\n- scope: schedule:read\n  description: Read class dates / schedules.\n- scope: schedule:write\n  description: Add and remove class dates (implies schedule:read).\n- scope: template:read\n  description: Read class templates.\n- scope: template:write\n  description: Create, update and remove class templates (implies template:read).\n- scope: user:read\n  description: Read non-learner users.\n- scope: user:write\n  description: Create, update and remove non-learner users (implies user:read).\nnotes:\n- >-\n  Scopes are attached to the API key rather than issued via an OAuth flow; this\n  is API-key authorization with a scope model, not OAuth 2.0.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/class-fka-classedu/refs/heads/main/authentication/class-fka-classedu-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Education
- EdTech
- Virtual Classroom
- Learning Management
- Online Learning
- Training
- Zoom
- Microsoft Teams
- Attendance
---
