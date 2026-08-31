---
api_key_in:
- header
api_specs:
- filename: zesty-instances-api-openapi.yml
  format: yaml
  label: Zesty Instances API
  slug: instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-instances-api-openapi.yml
- filename: zesty-apps-api-openapi.yml
  format: yaml
  label: Zesty Apps API
  slug: zesty-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-apps-api-openapi.yml
- filename: zesty-authentication-api-openapi.yml
  format: yaml
  label: Zesty Authentication API
  slug: zesty-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-authentication-api-openapi.yml
- filename: zesty-bins-api-openapi.yml
  format: yaml
  label: Zesty Bins API
  slug: zesty-bins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-bins-api-openapi.yml
- filename: zesty-files-api-openapi.yml
  format: yaml
  label: Zesty Files API
  slug: zesty-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-files-api-openapi.yml
- filename: zesty-groups-api-openapi.yml
  format: yaml
  label: Zesty Groups API
  slug: zesty-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-groups-api-openapi.yml
- filename: zesty-password-api-openapi.yml
  format: yaml
  label: Zesty Password API
  slug: zesty-password-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-password-api-openapi.yml
- filename: zesty-resolver-api-openapi.yml
  format: yaml
  label: Zesty Resolver API
  slug: zesty-resolver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-resolver-api-openapi.yml
- filename: zesty-roles-api-openapi.yml
  format: yaml
  label: Zesty Roles API
  slug: zesty-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-roles-api-openapi.yml
- filename: zesty-teams-api-openapi.yml
  format: yaml
  label: Zesty Teams API
  slug: zesty-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-teams-api-openapi.yml
- filename: zesty-tokens-api-openapi.yml
  format: yaml
  label: Zesty Tokens API
  slug: zesty-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-tokens-api-openapi.yml
- filename: zesty-users-api-openapi.yml
  format: yaml
  label: Zesty Users API
  slug: zesty-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-users-api-openapi.yml
- filename: zesty-webhooks-api-openapi.yml
  format: yaml
  label: Zesty Webhooks API
  slug: zesty-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/openapi/zesty-webhooks-api-openapi.yml
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
