---
api_key_in: []
api_specs:
- filename: fini-openapi.yml
  format: yaml
  label: Fini AI API
  slug: fini-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fini/refs/heads/main/openapi/fini-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fini Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fini secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fini
provider_slug: fini
scheme_count: 1
schemes:
- bearerFormat: fini_ API key
  description: 'Bearer token containing your Fini workspace API key. Format: `Bearer [example key]`. Every request to the public v2 API authenticates with a workspace API key sent as a bearer token. Keys carry coarse `read` and/or `write` scope; read routes require `read`, write/mutating routes require `write`. A key without the required scope returns 403 Forbidden with body {"statusCode":403,"message":"API key does not have the required scope for this operation","error":"Forbidden"}.'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  scopes:
  - description: Read/export routes (list and get conversations, sources, articles, folders, rules, tags, agents, prompts).
    name: read
  - description: Mutating routes (create/update/delete, ingest, generate knowledge, generate answer, publish, assign).
    name: write
  sources:
  - openapi/fini-openapi.yml
  type: http
slug: fini-authentication
source_filename: fini-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fini-openapi.yml\ndocs: https://docs.usefini.com/en/api-reference/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_format: fini_\n  api_key_scopes:\n  - read\n  - write\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: fini_ API key\n  in: header\n  header: Authorization\n  description: >-\n    Bearer token containing your Fini workspace API key. Format: `Bearer [example key]`. Every request\n    to the public v2 API authenticates with a workspace API key sent as a bearer token. Keys carry\n    coarse `read` and/or `write` scope; read routes require `read`, write/mutating routes require\n    `write`. A key without the required scope returns 403 Forbidden with body\n    {\"statusCode\":403,\"message\":\"API key does not have the required scope for this operation\",\"error\":\"Forbidden\"}.\n  scopes:\n  - name: read\n    description: Read/export routes (list\
  \ and get conversations, sources, articles, folders, rules, tags, agents, prompts).\n  - name: write\n    description: Mutating routes (create/update/delete, ingest, generate knowledge, generate answer, publish, assign).\n  sources:\n  - openapi/fini-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fini/refs/heads/main/authentication/fini-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Agents
- Customer Support
- Customer Experience
- Knowledge Management
- Conversational AI
- Voice AI
- Helpdesk
- Regulated Industries
---
