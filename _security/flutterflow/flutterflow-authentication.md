---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Flutterflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: FlutterFlow secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FlutterFlow
provider_slug: flutterflow
scheme_count: 1
schemes:
- bearer_format: FlutterFlow API token
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - docs
  token_management:
    cli_env: FLUTTERFLOW_API_TOKEN
    credentials_file: ~/.flutterflow/credentials.json
  type: http
  value_format: Bearer <FLUTTERFLOW_API_TOKEN>
slug: flutterflow-authentication
source_filename: flutterflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.flutterflow.io/resources/projects/settings/project-apis/\ndocs: https://docs.flutterflow.io/resources/projects/settings/project-apis/\nnotes: >-\n  FlutterFlow has no published OpenAPI for its Project APIs, so this profile is\n  captured from the documentation rather than derived from a securityScheme. All\n  Project API endpoints require a Bearer FlutterFlow API token in the Authorization\n  header. The same token authenticates the flutterflow_cli client and the AI MCP\n  server. There is no OAuth / scope surface.\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  oauth2: false\n  api_key_in: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: FlutterFlow API token\n  in: header\n  header: Authorization\n  value_format: 'Bearer <FLUTTERFLOW_API_TOKEN>'\n  token_management:\n    cli_env: FLUTTERFLOW_API_TOKEN\n    credentials_file: ~/.flutterflow/credentials.json\n  sources:\
  \ [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flutterflow/refs/heads/main/authentication/flutterflow-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Developer Tools
- Low-Code
- No-Code
- App Builder
- Flutter
- Mobile Development
- Visual Development
- API
- CLI
- MCP
---
