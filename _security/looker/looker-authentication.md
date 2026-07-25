---
api_key_in: []
api_specs:
- filename: looker-auth-api-openapi.yml
  format: yaml
  label: Looker Auth API
  slug: looker-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/openapi/looker-auth-api-openapi.yml
- filename: looker-dashboard-api-openapi.yml
  format: yaml
  label: Looker Dashboard API
  slug: looker-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/openapi/looker-dashboard-api-openapi.yml
- filename: looker-look-api-openapi.yml
  format: yaml
  label: Looker Look API
  slug: looker-look-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/openapi/looker-look-api-openapi.yml
- filename: looker-query-api-openapi.yml
  format: yaml
  label: Looker Query API
  slug: looker-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/openapi/looker-query-api-openapi.yml
- filename: looker-user-api-openapi.yml
  format: yaml
  label: Looker User API
  slug: looker-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/openapi/looker-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Looker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Looker secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Looker
provider_slug: looker
scheme_count: 1
schemes:
- description: Access token obtained from the /login endpoint using client credentials. Include as Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/looker-api-openapi.yml
  type: http
slug: looker-authentication
source_filename: looker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/looker-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Access token obtained from the /login endpoint using client credentials. Include\n    as Bearer token in the Authorization header.\n  sources:\n  - openapi/looker-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/authentication/looker-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
---
