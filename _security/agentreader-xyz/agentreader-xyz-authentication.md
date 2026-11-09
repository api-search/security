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
name: Agentreader Xyz Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentReader secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AgentReader
provider_slug: agentreader-xyz
scheme_count: 1
schemes:
- description: Optional API key holding prepaid credits (ar_...)
  name: bearerApiKey
  scheme: bearer
  sources:
  - openapi/agentreader-xyz-openapi.json
  type: http
slug: agentreader-xyz-authentication
source_filename: agentreader-xyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/agentreader-xyz-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  description: Optional API key holding prepaid credits (ar_...)\n  sources:\n  - openapi/agentreader-xyz-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/agentreader-xyz/authentication/agentreader-xyz-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Data Processing
- PDF
- Markdown
- Agent Tools
---
