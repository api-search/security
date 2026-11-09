---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agenticrail-nz-enforcement-api-openapi.yml
  format: yaml
  label: AgenticRail Enforcement API
  slug: agenticrail-nz-enforcement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticrail-nz/openapi/agenticrail-nz-enforcement-api-openapi.yml
- filename: agenticrail-nz-evidence-api-openapi.yml
  format: yaml
  label: AgenticRail Evidence API
  slug: agenticrail-nz-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticrail-nz/openapi/agenticrail-nz-evidence-api-openapi.yml
- filename: agenticrail-nz-operational-api-openapi.yml
  format: yaml
  label: AgenticRail Operational API
  slug: agenticrail-nz-operational-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticrail-nz/openapi/agenticrail-nz-operational-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Agenticrail Nz Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgenticRail secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AgenticRail
provider_slug: agenticrail-nz
scheme_count: 1
schemes:
- description: '`Authorization: Bearer <your-key>`. Optional.


    An UNRECOGNISED identity is served on the public demo lane rather than refused: no header at all, a string that cannot be a key, or a well-formed prefix that was never issued. The call runs, the receipt is real, and the response carries `lane`, `lane_reason` and `lane_notice` saying so.


    A KNOWN identity presented wrongly is still refused: a wrong sec'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/agenticrail-nz-openapi.json
  type: http
slug: agenticrail-nz-authentication
source_filename: agenticrail-nz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/agenticrail-nz-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    `Authorization: Bearer <your-key>`. Optional.\n\n    An UNRECOGNISED identity is served on the public demo lane rather than refused: no header at all, a string that cannot be a key, or a well-formed prefix that was never issued. The call runs, the receipt is real, and the response carries `lane`, `lane_reason` and `lane_notice` saying so.\n\n    A KNOWN identity presented wrongly is still refused: a wrong sec\n  sources:\n  - openapi/agenticrail-nz-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/agenticrail-nz/authentication/agenticrail-nz-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Automation
- Sequence Enforcement
- Cryptographic Receipts
- Compliance
---
