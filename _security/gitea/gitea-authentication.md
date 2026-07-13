---
api_key_in:
- header
- query
api_specs:
- filename: swagger.v1.json
  format: json
  label: Gitea REST API
  slug: gitea-rest-api
  spec_type: OpenAPI
  url: https://demo.gitea.com/swagger.v1.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gitea Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gitea secures its APIs with apiKey and http across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gitea
provider_slug: gitea
scheme_count: 7
schemes:
- description: This authentication option is deprecated for removal in Gitea 1.23. Please use AuthorizationHeaderToken instead.
  in: query
  name: AccessToken
  parameter: access_token
  sources:
  - openapi/gitea-rest-api-openapi-original.yml
  - openapi/gitea-rest-api-openapi.yml
  type: apiKey
- description: API tokens must be prepended with "token" followed by a space.
  in: header
  name: AuthorizationHeaderToken
  parameter: Authorization
  sources:
  - openapi/gitea-rest-api-openapi-original.yml
  - openapi/gitea-rest-api-openapi.yml
  type: apiKey
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/gitea-rest-api-openapi-original.yml
  - openapi/gitea-rest-api-openapi.yml
  type: http
- description: Sudo API request as the user provided as the key. Admin privileges are required.
  in: header
  name: SudoHeader
  parameter: Sudo
  sources:
  - openapi/gitea-rest-api-openapi-original.yml
  - openapi/gitea-rest-api-openapi.yml
  type: apiKey
- description: Sudo API request as the user provided as the key. Admin privileges are required.
  in: query
  name: SudoParam
  parameter: sudo
  sources:
  - openapi/gitea-rest-api-openapi-original.yml
  - openapi/gitea-rest-api-openapi.yml
  type: apiKey
- description: Must be used in combination with BasicAuth if two-factor authentication is enabled.
  in: header
  name: TOTPHeader
  parameter: X-GITEA-OTP
  sources:
  - openapi/gitea-rest-api-openapi-original.yml
  - openapi/gitea-rest-api-openapi.yml
  type: apiKey
- description: This authentication option is deprecated for removal in Gitea 1.23. Please use AuthorizationHeaderToken instead.
  in: query
  name: Token
  parameter: token
  sources:
  - openapi/gitea-rest-api-openapi-original.yml
  - openapi/gitea-rest-api-openapi.yml
  type: apiKey
slug: gitea-authentication
source_filename: gitea-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gitea-rest-api-openapi-original.yml, openapi/gitea-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: AccessToken\n  type: apiKey\n  in: query\n  parameter: access_token\n  description: This authentication option is deprecated for removal in Gitea 1.23. Please use\n    AuthorizationHeaderToken instead.\n  sources:\n  - openapi/gitea-rest-api-openapi-original.yml\n  - openapi/gitea-rest-api-openapi.yml\n- name: AuthorizationHeaderToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API tokens must be prepended with \"token\" followed by a space.\n  sources:\n  - openapi/gitea-rest-api-openapi-original.yml\n  - openapi/gitea-rest-api-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/gitea-rest-api-openapi-original.yml\n  - openapi/gitea-rest-api-openapi.yml\n- name: SudoHeader\n  type: apiKey\n\
  \  in: header\n  parameter: Sudo\n  description: Sudo API request as the user provided as the key. Admin privileges are required.\n  sources:\n  - openapi/gitea-rest-api-openapi-original.yml\n  - openapi/gitea-rest-api-openapi.yml\n- name: SudoParam\n  type: apiKey\n  in: query\n  parameter: sudo\n  description: Sudo API request as the user provided as the key. Admin privileges are required.\n  sources:\n  - openapi/gitea-rest-api-openapi-original.yml\n  - openapi/gitea-rest-api-openapi.yml\n- name: TOTPHeader\n  type: apiKey\n  in: header\n  parameter: X-GITEA-OTP\n  description: Must be used in combination with BasicAuth if two-factor authentication is enabled.\n  sources:\n  - openapi/gitea-rest-api-openapi-original.yml\n  - openapi/gitea-rest-api-openapi.yml\n- name: Token\n  type: apiKey\n  in: query\n  parameter: token\n  description: This authentication option is deprecated for removal in Gitea 1.23. Please use\n    AuthorizationHeaderToken instead.\n  sources:\n  - openapi/gitea-rest-api-openapi-original.yml\n\
  \  - openapi/gitea-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitea/refs/heads/main/authentication/gitea-authentication.yml
summary_line: apiKey/http · 7 schemes
tags:
- Git
- Source Control
- DevOps
- CI/CD
- Code Hosting
- Open Source
- Self Hosted
- Package Registry
- Issue Tracking
- Pull Requests
---
