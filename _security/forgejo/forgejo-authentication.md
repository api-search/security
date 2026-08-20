---
api_key_in:
- header
- query
api_specs:
- filename: forgejo-activitypub-api-openapi.yml
  format: yaml
  label: Forgejo activitypub API
  slug: forgejo-activitypub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-activitypub-api-openapi.yml
- filename: forgejo-admin-api-openapi.yml
  format: yaml
  label: Forgejo admin API
  slug: forgejo-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-admin-api-openapi.yml
- filename: forgejo-issue-api-openapi.yml
  format: yaml
  label: Forgejo issue API
  slug: forgejo-issue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-issue-api-openapi.yml
- filename: forgejo-miscellaneous-api-openapi.yml
  format: yaml
  label: Forgejo miscellaneous API
  slug: forgejo-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-miscellaneous-api-openapi.yml
- filename: forgejo-notification-api-openapi.yml
  format: yaml
  label: Forgejo notification API
  slug: forgejo-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-notification-api-openapi.yml
- filename: forgejo-organization-api-openapi.yml
  format: yaml
  label: Forgejo organization API
  slug: forgejo-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-organization-api-openapi.yml
- filename: forgejo-package-api-openapi.yml
  format: yaml
  label: Forgejo package API
  slug: forgejo-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-package-api-openapi.yml
- filename: forgejo-repository-api-openapi.yml
  format: yaml
  label: Forgejo repository API
  slug: forgejo-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-repository-api-openapi.yml
- filename: forgejo-settings-api-openapi.yml
  format: yaml
  label: Forgejo settings API
  slug: forgejo-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-settings-api-openapi.yml
- filename: forgejo-user-api-openapi.yml
  format: yaml
  label: Forgejo user API
  slug: forgejo-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/openapi/forgejo-user-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Forgejo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forgejo secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Forgejo
provider_slug: forgejo
scheme_count: 5
schemes:
- description: API tokens must be prepended with "token" followed by a space.
  in: header
  name: AuthorizationHeaderToken
  parameter: Authorization
  sources:
  - openapi/openapi.json
  type: apiKey
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/openapi.json
  type: http
- description: Sudo API request as the user provided as the key. Admin privileges are required.
  in: header
  name: SudoHeader
  parameter: Sudo
  sources:
  - openapi/openapi.json
  type: apiKey
- description: Sudo API request as the user provided as the key. Admin privileges are required.
  in: query
  name: SudoParam
  parameter: sudo
  sources:
  - openapi/openapi.json
  type: apiKey
- description: Must be used in combination with BasicAuth if two-factor authentication is enabled.
  in: header
  name: TOTPHeader
  parameter: X-FORGEJO-OTP
  sources:
  - openapi/openapi.json
  type: apiKey
slug: forgejo-authentication
source_filename: forgejo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: AuthorizationHeaderToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API tokens must be prepended with \"token\" followed by a space.\n  sources:\n  - openapi/openapi.json\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/openapi.json\n- name: SudoHeader\n  type: apiKey\n  in: header\n  parameter: Sudo\n  description: Sudo API request as the user provided as the key. Admin privileges are required.\n  sources:\n  - openapi/openapi.json\n- name: SudoParam\n  type: apiKey\n  in: query\n  parameter: sudo\n  description: Sudo API request as the user provided as the key. Admin privileges are required.\n  sources:\n  - openapi/openapi.json\n- name: TOTPHeader\n  type: apiKey\n  in: header\n  parameter: X-FORGEJO-OTP\n  description: Must be used in combination\
  \ with BasicAuth if two-factor authentication is enabled.\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forgejo/refs/heads/main/authentication/forgejo-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Git
- Source Code Management
- Self-Hosted
- DevOps
- CI/CD
- Open-Source
- Forge
- Repositories
- Issues
- Pull Requests
---
