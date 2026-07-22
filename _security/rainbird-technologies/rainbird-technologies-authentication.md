---
api_key_in:
- header
api_specs:
- filename: rainbird-technologies-openapi-original.json
  format: json
  label: Rainbird API
  slug: rainbird-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbird-technologies/refs/heads/main/openapi/rainbird-technologies-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Rainbird Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rainbird Technologies secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rainbird Technologies
provider_slug: rainbird-technologies
scheme_count: 3
schemes:
- description: "Authentication with the Rainbird API uses a user key, passed in the header. This can be found on the Account page or with the controls for [publishing a Knowledge Map](https://docs.rainbird.ai/rainbird/knowledge-modelling/publishing-your-km/api-management).  \n\nOur legacy authentication method of HTTP BasicAuth continues to be supported, but we highly advise transitioning to the new method."
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/rainbird-technologies-openapi-original.json
  type: apiKey
- description: To access secured evidence, you should pass your evidence key
  in: header
  name: evidenceKey
  parameter: x-evidence-key
  sources:
  - openapi/rainbird-technologies-openapi-original.json
  type: apiKey
- description: To access secured interaction logs, you should pass your interaction key
  in: header
  name: interactionKey
  parameter: x-interaction-key
  sources:
  - openapi/rainbird-technologies-openapi-original.json
  type: apiKey
slug: rainbird-technologies-authentication
source_filename: rainbird-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/rainbird-technologies-openapi-original.json\ndocs: https://docs.rainbird.ai/rainbird/knowledge-modelling/publishing-your-km/api-management\nnotes: >-\n  Primary auth is the X-API-Key header (obtained from the KM Publish panel or Account\n  page). Evidence and interaction data require additional x-evidence-key / x-interaction-key\n  headers unless link-sharing is enabled. Legacy HTTP BasicAuth remains supported but deprecated.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: \"Authentication with the Rainbird API uses a user key, passed in the header.\\\n    \\ This can be found on the Account page or with the controls for [publishing a Knowledge\\\n    \\ Map](https://docs.rainbird.ai/rainbird/knowledge-modelling/publishing-your-km/api-management).\\\n    \\  \\n\\nOur legacy authentication method of HTTP BasicAuth\
  \ continues to be supported, but\\\n    \\ we highly advise transitioning to the new method.\"\n  sources:\n  - openapi/rainbird-technologies-openapi-original.json\n- name: evidenceKey\n  type: apiKey\n  in: header\n  parameter: x-evidence-key\n  description: To access secured evidence, you should pass your evidence key\n  sources:\n  - openapi/rainbird-technologies-openapi-original.json\n- name: interactionKey\n  type: apiKey\n  in: header\n  parameter: x-interaction-key\n  description: To access secured interaction logs, you should pass your interaction key\n  sources:\n  - openapi/rainbird-technologies-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainbird-technologies/refs/heads/main/authentication/rainbird-technologies-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Artificial Intelligence
- Decision Automation
- Knowledge Graph
- Symbolic Reasoning
- Explainable AI
- Governance
- RegTech
---
