---
api_key_in: []
api_specs:
- filename: open-webui-openapi.yml
  format: yaml
  label: Open WebUI API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-webui/refs/heads/main/openapi/open-webui-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Open Webui Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open WebUI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Open WebUI
provider_slug: open-webui
scheme_count: 1
schemes:
- description: 'Bearer token: Open WebUI session token or per-user API key. Each API key

    inherits the permissions of the user who created it.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/open-webui-openapi.yml
  type: http
slug: open-webui-authentication
source_filename: open-webui-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/open-webui-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer token: Open WebUI session token or per-user API key. Each API key\n    inherits the permissions of the user who created it.\n  sources:\n  - openapi/open-webui-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-webui/refs/heads/main/authentication/open-webui-authentication.yml
summary_line: http · 1 scheme
tags:
- LLM
- Open Source
- Self-Hosted
- Ollama
- Chat UI
- RAG
---
