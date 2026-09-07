---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: striim-tql-files-rest-api-5-4-0-2-openapi.yml
  format: yaml
  label: Striim Application Management REST API
  slug: striim-application-management-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/striim/refs/heads/main/openapi/striim-tql-files-rest-api-5-4-0-2-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Striim Authentication
name_suffix: Authentication
oauth_flows: []
overview: Striim secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Striim
provider_slug: striim
scheme_count: 1
schemes:
- description: 'A 36-character authentication token must be included in all API calls, sent as "Authorization: STRIIM-TOKEN <token>". Tokens are obtained from the Striim Cloud Console (Services > More > API) or programmatically via a REST login call.'
  format: STRIIM-TOKEN <36-character token>
  in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/striim-application-management-rest-api-3-10-1-openapi.yml
  - openapi/striim-application-management-rest-api-3-10-3-openapi.yml
  - openapi/striim-tql-files-rest-api-5-4-0-2-openapi.yml
  type: apiKey
slug: striim-authentication
source_filename: striim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: openapi/striim-application-management-rest-api-3-10-1-openapi.yml, openapi/striim-application-management-rest-api-3-10-3-openapi.yml,\n  openapi/striim-tql-files-rest-api-5-4-0-2-openapi.yml ; Authorization article (striim.stoplight.io/docs/striim-application-management/ZG9jOjUxODM1Mjk-authorization)\n  ; https://www.striim.com/docs/en/api-guide.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/striim-application-management-rest-api-3-10-1-openapi.yml\n  - openapi/striim-application-management-rest-api-3-10-3-openapi.yml\n  - openapi/striim-tql-files-rest-api-5-4-0-2-openapi.yml\n  format: STRIIM-TOKEN <36-character token>\n  description: 'A 36-character authentication token must be included in all API calls, sent as \"Authorization: STRIIM-TOKEN\n    <token>\". Tokens are obtained from the Striim\
  \ Cloud Console (Services > More > API) or programmatically via\n    a REST login call.'\ndocs: https://www.striim.com/docs/en/api-guide.html\nnotes: The API also accepts the token as a `token` query parameter per the API Guide, but the OpenAPI definitions\n  declare only the Authorization header scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/striim/refs/heads/main/authentication/striim-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data
- Streaming
- Change Data Capture
- Real-Time
- Data Integration
- Streaming Analytics
---
