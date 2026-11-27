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
name: Lumind Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lumind secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lumind
provider_slug: lumind-io
scheme_count: 1
schemes:
- description: 'Agent key issued by the owner: `Authorization: Bearer lmd_agent_...`'
  name: agentKey
  scheme: bearer
  sources:
  - openapi/lumind-io-openapi.json
  type: http
slug: lumind-io-authentication
source_filename: lumind-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/lumind-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: agentKey\n  type: http\n  scheme: bearer\n  description: 'Agent key issued by the owner: `Authorization: Bearer lmd_agent_...`'\n  sources:\n  - openapi/lumind-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lumind-io/authentication/lumind-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Managed Service
- Automation
- Multilingual
- Customer Service
---
