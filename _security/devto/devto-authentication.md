---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: DEV Community API
  slug: devto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Devto Authentication
name_suffix: Authentication
oauth_flows: []
overview: DEV Community secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DEV Community
provider_slug: devto
scheme_count: 1
schemes:
- description: "API Key authentication.\n\nAuthentication for some endpoints, like write operations on the\nArticles API require a DEV API key.\n\nAll authenticated endpoints are CORS disabled, the API key is intended for non-browser scripts.\n\n### Getting an API key\n\nTo obtain one, please follow these steps:\n\n  - visit https://dev.to/settings/extensions\n  - in the \"DEV API Keys\" section create a new key by adding a\n  "
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/openapi.json
  - openapi/openapi.yaml
  type: apiKey
slug: devto-authentication
source_filename: devto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json, openapi/openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: \"API Key authentication.\\n\\nAuthentication for some endpoints, like write operations\\\n    \\ on the\\nArticles API require a DEV API key.\\n\\nAll authenticated endpoints are CORS disabled,\\\n    \\ the API key is intended for non-browser scripts.\\n\\n### Getting an API key\\n\\nTo obtain\\\n    \\ one, please follow these steps:\\n\\n  - visit https://dev.to/settings/extensions\\n  - in\\\n    \\ the \\\"DEV API Keys\\\" section create a new key by adding a\\n  \"\n  sources:\n  - openapi/openapi.json\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/authentication/devto-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Developer Community
- Articles
- Blogging
- Social
- Content
- Open Source
---
