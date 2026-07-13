---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openhands Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenHands secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenHands
provider_slug: openhands
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-Session-API-Key
  sources:
  - openapi/openhands-openapi.json
  type: apiKey
slug: openhands-authentication
source_filename: openhands-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openhands-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Session-API-Key\n  sources:\n  - openapi/openhands-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openhands/refs/heads/main/authentication/openhands-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Agents
- Autonomous
- Open Source
- Developer Tools
- Software Engineering
- Code Generation
---
