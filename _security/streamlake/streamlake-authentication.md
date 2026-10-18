---
anonymous_access: false
api_key_in: []
api_specs:
- filename: streamlake-gateway-api-openapi.yml
  format: yaml
  label: StreamLake Gateway API
  slug: streamlake-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamlake/refs/heads/main/openapi/streamlake-gateway-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Streamlake Authentication
name_suffix: Authentication
oauth_flows: []
overview: StreamLake declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: StreamLake
provider_slug: streamlake
scheme_count: 1
schemes:
- description: API keys are created and managed in the Vanchin Console (Vanchin Console > API Key), which shows a system default key and lets users create and delete custom keys; deletion is permanent.
  format: 'Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  in: header
  name: bearer
  scheme: bearer
  type: http
slug: streamlake-authentication
source_filename: streamlake-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: StreamLake Vanchin API Authentication\ngenerated: '2026-10-13'\nmethod: searched\nsource: https://streamlake.ai/document/DOC/mj9z6fh8lxn87i86jrp\ndocs: https://streamlake.ai/document/DOC/mkaylxzkso38sqxcpa\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer YOUR_API_KEY'\n  description: API keys are created and managed in the Vanchin Console (Vanchin Console > API Key), which shows a system default key and lets users create and delete custom keys; deletion is permanent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamlake/refs/heads/main/authentication/streamlake-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- LLM
- Model Inference
- Chat Completions
- AI Coding
- Kuaishou
---
