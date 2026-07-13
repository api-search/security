---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Height REST API
  slug: height-api
  spec_type: OpenAPI
  url: https://height-api.xyz/openapi/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Height Authentication
name_suffix: Authentication
oauth_flows: []
overview: Height secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Height
provider_slug: height
scheme_count: 1
schemes:
- description: "The Height API uses API keys to authenticate requests. **You can view your API key in the Height settings under API**.\n ex: `api-key secret_1234`"
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/height-height-api-openapi.yml
  type: apiKey
slug: height-authentication
source_filename: height-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/height-height-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    The Height API uses API keys to authenticate requests. **You can view your API key in the Height settings under API**.\n     ex: `api-key secret_1234`\n  sources:\n  - openapi/height-height-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/authentication/height-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Project Management
- Task Management
- Collaboration
- Productivity
- Workflow Automation
- AI
---
