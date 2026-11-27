---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clawdcall-com-cc-api-openapi.yml
  format: yaml
  label: ClawdCall Cc API
  slug: clawdcall-com-cc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawdcall-com/openapi/clawdcall-com-cc-api-openapi.yml
- filename: clawdcall-com-external-api-openapi.yml
  format: yaml
  label: ClawdCall External API
  slug: clawdcall-com-external-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clawdcall-com/openapi/clawdcall-com-external-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: ClawdCall Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClawdCall secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ClawdCall
provider_slug: clawdcall-com
scheme_count: 1
schemes:
- description: ClawdCall API key obtained through the signup and phone verification flow in /skill.md.
  name: bearerApiKey
  scheme: bearer
  sources:
  - openapi/clawdcall-com-openapi.json
  type: http
slug: clawdcall-com-authentication
source_filename: clawdcall-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/clawdcall-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  description: ClawdCall API key obtained through the signup and phone verification flow in\n    /skill.md.\n  sources:\n  - openapi/clawdcall-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/clawdcall-com/authentication/clawdcall-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Voice
- Automation
- Agents
- Telephony
---
