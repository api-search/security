---
api_key_in: []
api_specs:
- filename: hatch-openapi-original.json
  format: json
  label: Hatch API
  slug: hatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hatch/refs/heads/main/openapi/hatch-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hatch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hatch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hatch
provider_slug: hatch
scheme_count: 1
schemes:
- format: 'Authorization: Bearer <api_key>'
  header: Authorization
  in: header
  name: authorization
  scheme: bearer
  sources:
  - openapi/hatch-openapi-original.json
  type: http
slug: hatch-authentication
source_filename: hatch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/hatch-openapi-original.json\ndocs: https://docs.usehatchapp.com/integrations/hatch-api/hatch-api-reference\nsummary:\n  types:\n  - http\n  scheme: bearer\n  token_type: api-key\n  token_management: >-\n    API keys are created and managed in the API Keys tab of the App Marketplace\n    on the Hatch platform. Keys are passed as an HTTP bearer token.\nschemes:\n- name: authorization\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <api_key>'\n  sources:\n  - openapi/hatch-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hatch/refs/heads/main/authentication/hatch-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Vertical Software
- Customer Communication
- Conversational AI
- SMS
- Voice
- Email
- Marketing
- Home Services
- Contact Center
---
