---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Promptzone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Promptzone secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Promptzone
provider_slug: promptzone
scheme_count: 2
schemes:
- description: "API Key authentication.\n\nAuthentication for some endpoints, like write operations on the\nArticles API require a DEV API key.\n\nAll authenticated endpoints are CORS disabled, the API key is intended for non-browser scripts.\n\n### Getting an API key\n\nTo obtain one, please follow these steps:\n\n  - visit https://dev.to/settings/extensions\n  - in the \"DEV API Keys\" section create a new key by adding a\n  "
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/promptzone-openapi.json
  type: apiKey
- bearerFormat: JWT
  description: Short-lived RS256 RFC 9068 access token issued by the configured delegation service and verified against its configured JWKS. The issuer authorizes the client and requested operation before minting the token; Forem validates the token and resolves its subject and owner to a local user. An invalid token returns 401; an unavailable trust dependency with no usable cached key returns 503.
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/promptzone-openapi.json
  type: http
slug: promptzone-authentication
source_filename: promptzone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/promptzone-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: \"API Key authentication.\\n\\nAuthentication for some endpoints, like write operations\\\n    \\ on the\\nArticles API require a DEV API key.\\n\\nAll authenticated endpoints are CORS disabled,\\\n    \\ the API key is intended for non-browser scripts.\\n\\n### Getting an API key\\n\\nTo obtain\\\n    \\ one, please follow these steps:\\n\\n  - visit https://dev.to/settings/extensions\\n  - in\\\n    \\ the \\\"DEV API Keys\\\" section create a new key by adding a\\n  \"\n  sources:\n  - openapi/promptzone-openapi.json\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Short-lived RS256 RFC 9068 access token issued by the configured delegation service\n    and verified against its configured JWKS.\
  \ The issuer authorizes the client and requested\n    operation before minting the token; Forem validates the token and resolves its subject and\n    owner to a local user. An invalid token returns 401; an unavailable trust dependency with\n    no usable cached key returns 503.\n  sources:\n  - openapi/promptzone-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/promptzone/authentication/promptzone-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Community
- Prompts
- Tools
- Resources
---
