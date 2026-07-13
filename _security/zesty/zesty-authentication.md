---
api_key_in:
- header
api_specs:
- filename: zesty-auth-api-openapi.yml
  format: yaml
  label: Zesty Auth API
  slug: auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-auth-api-openapi.yml
- filename: zesty-accounts-api-openapi.yml
  format: yaml
  label: Zesty Accounts API
  slug: accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-accounts-api-openapi.yml
- filename: zesty-instances-api-openapi.yml
  format: yaml
  label: Zesty Instances API
  slug: instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-instances-api-openapi.yml
- filename: zesty-media-api-openapi.yml
  format: yaml
  label: Zesty Media API
  slug: media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-media-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Zesty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zesty secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zesty
provider_slug: zesty
scheme_count: 1
schemes:
- description: A session token obtained from the Auth API login endpoint.
  in: header
  name: sessionToken
  parameter: Authorization
  sources:
  - openapi/zesty-accounts-api-openapi.yml
  - openapi/zesty-auth-api-openapi.yml
  - openapi/zesty-instances-api-openapi.yml
  - openapi/zesty-media-api-openapi.yml
  type: apiKey
slug: zesty-authentication
source_filename: zesty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zesty-accounts-api-openapi.yml, openapi/zesty-auth-api-openapi.yml, openapi/zesty-instances-api-openapi.yml,\n  openapi/zesty-media-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sessionToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: A session token obtained from the Auth API login endpoint.\n  sources:\n  - openapi/zesty-accounts-api-openapi.yml\n  - openapi/zesty-auth-api-openapi.yml\n  - openapi/zesty-instances-api-openapi.yml\n  - openapi/zesty-media-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/authentication/zesty-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CMS
- Composable
- Content Management
- GraphQL
- Headless CMS
- Media
---
