---
api_key_in: []
api_specs:
- filename: appmixer-accounts-api-openapi.yml
  format: yaml
  label: Appmixer Accounts API
  slug: appmixer-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-accounts-api-openapi.yml
- filename: appmixer-apps-api-openapi.yml
  format: yaml
  label: Appmixer Apps API
  slug: appmixer-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-apps-api-openapi.yml
- filename: appmixer-authentication-api-openapi.yml
  format: yaml
  label: Appmixer Authentication API
  slug: appmixer-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-authentication-api-openapi.yml
- filename: appmixer-data-stores-api-openapi.yml
  format: yaml
  label: Appmixer Data Stores API
  slug: appmixer-data-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-data-stores-api-openapi.yml
- filename: appmixer-files-api-openapi.yml
  format: yaml
  label: Appmixer Files API
  slug: appmixer-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-files-api-openapi.yml
- filename: appmixer-flows-api-openapi.yml
  format: yaml
  label: Appmixer Flows API
  slug: appmixer-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-flows-api-openapi.yml
- filename: appmixer-insights-api-openapi.yml
  format: yaml
  label: Appmixer Insights API
  slug: appmixer-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-insights-api-openapi.yml
- filename: appmixer-logs-api-openapi.yml
  format: yaml
  label: Appmixer Logs API
  slug: appmixer-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-logs-api-openapi.yml
- filename: appmixer-messages-api-openapi.yml
  format: yaml
  label: Appmixer Messages API
  slug: appmixer-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-messages-api-openapi.yml
- filename: appmixer-people-tasks-api-openapi.yml
  format: yaml
  label: Appmixer People Tasks API
  slug: appmixer-people-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-people-tasks-api-openapi.yml
- filename: appmixer-system-api-openapi.yml
  format: yaml
  label: Appmixer System API
  slug: appmixer-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-system-api-openapi.yml
- filename: appmixer-users-api-openapi.yml
  format: yaml
  label: Appmixer Users API
  slug: appmixer-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Appmixer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appmixer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Appmixer
provider_slug: appmixer
scheme_count: 1
schemes:
- description: 'Access token obtained from the /user/auth endpoint. Pass as Authorization: Bearer {token} header.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/appmixer-api-openapi.yml
  type: http
slug: appmixer-authentication
source_filename: appmixer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/appmixer-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Access token obtained from the /user/auth endpoint. Pass as Authorization: Bearer\n    {token} header.'\n  sources:\n  - openapi/appmixer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/authentication/appmixer-authentication.yml
summary_line: http · 1 scheme
tags:
- Agentic
- Automation
- Embedded iPaaS
- Integrations
- Low-Code
- Workflows
---
