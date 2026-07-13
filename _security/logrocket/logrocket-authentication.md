---
api_key_in:
- header
api_specs:
- filename: logrocket-rest-api-openapi.yml
  format: yaml
  label: LogRocket REST API
  slug: logrocket-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logrocket/refs/heads/main/openapi/logrocket-rest-api-openapi.yml
- filename: logrocket-graphql-api-openapi.yml
  format: yaml
  label: LogRocket GraphQL API
  slug: logrocket-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logrocket/refs/heads/main/openapi/logrocket-graphql-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Logrocket Authentication
name_suffix: Authentication
oauth_flows: []
overview: LogRocket secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LogRocket
provider_slug: logrocket
scheme_count: 1
schemes:
- description: API token authentication. Use the format "token <your-api-key>". API keys are available from the LogRocket dashboard under Settings > General Settings.
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/logrocket-graphql-api-openapi.yml
  - openapi/logrocket-rest-api-openapi.yml
  type: apiKey
slug: logrocket-authentication
source_filename: logrocket-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/logrocket-graphql-api-openapi.yml, openapi/logrocket-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API token authentication. Use the format \"token <your-api-key>\". API keys are\n    available from the LogRocket dashboard under Settings > General Settings.\n  sources:\n  - openapi/logrocket-graphql-api-openapi.yml\n  - openapi/logrocket-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logrocket/refs/heads/main/authentication/logrocket-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Session Replay
- Product Analytics
- Frontend Monitoring
- Logging
- Errors
---
