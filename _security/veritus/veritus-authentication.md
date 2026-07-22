---
api_key_in: []
api_specs:
- filename: veritus-openapi.json
  format: json
  label: Veritus API
  slug: veritus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veritus/refs/heads/main/openapi/veritus-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Veritus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veritus secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Veritus
provider_slug: veritus
scheme_count: 1
schemes:
- environment_scoped: true
  header: 'Authorization: Bearer <key>'
  issuance: Keys are provisioned directly by Veritus and cannot be self-regenerated; if lost or compromised a new key must be requested.
  key_format: Static secret key with an `sk-` prefix.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/veritus-openapi.json
  - https://docs.veritus.com/guides/authentication
  type: http
slug: veritus-authentication
source_filename: veritus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.veritus.com/guides/authentication\ndocs: https://docs.veritus.com/guides/authentication\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  key_format: Static secret key with an `sk-` prefix.\n  header: 'Authorization: Bearer <key>'\n  issuance: Keys are provisioned directly by Veritus and cannot be self-regenerated; if lost or compromised a new key must be requested.\n  environment_scoped: true\n  sources:\n  - openapi/veritus-openapi.json\n  - https://docs.veritus.com/guides/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veritus/refs/heads/main/authentication/veritus-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Consumer Lending
- Collections
- AI Agents
- Voice AI
- Communications
- Compliance
---
