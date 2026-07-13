---
api_key_in:
- cookie
- query
api_specs:
- filename: clerk-backend-api-openapi.yml
  format: yaml
  label: Clerk Backend API
  slug: clerk-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-com/refs/heads/main/openapi/clerk-backend-api-openapi.yml
- filename: clerk-frontend-api-openapi.yml
  format: yaml
  label: Clerk Frontend API
  slug: clerk-frontend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-com/refs/heads/main/openapi/clerk-frontend-api-openapi.yml
- filename: clerk-platform-api-openapi.yml
  format: yaml
  label: Clerk Platform API
  slug: clerk-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-com/refs/heads/main/openapi/clerk-platform-api-openapi.yml
- filename: clerk-webhooks-openapi.yml
  format: yaml
  label: Clerk Webhooks
  slug: clerk-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clerk-com/refs/heads/main/openapi/clerk-webhooks-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Clerk Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clerk secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clerk
provider_slug: clerk-com
scheme_count: 5
schemes:
- bearerFormat: sk_<environment>_<secret value>
  description: Secret key, obtained under "API Keys" in the Clerk Dashboard.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/clerk-backend-api-openapi.yml
  - openapi/clerk-frontend-api-openapi.yml
  - openapi/clerk-platform-api-openapi.yml
  type: http
- description: 'The Client API token sent in the form of a browser cookie.


    Used to authenticate production browser applications.'
  in: cookie
  name: ProductionBrowser
  parameter: __client
  sources:
  - openapi/clerk-frontend-api-openapi.yml
  type: apiKey
- description: 'A Dev Browser API token sent as a query parameter.


    Used to authenticate only dev instances.


    To generate a dev instance API token you must first make a request to `/v1/dev_browser`

    and copy it from the response.'
  in: query
  name: DevBrowser
  parameter: __dev_session
  sources:
  - openapi/clerk-frontend-api-openapi.yml
  type: apiKey
- description: 'If sent and the value is true, it instructs the server to parse the API token from the `Authorization` header.


    It should always be set to true when using the `Authorization` header authentication strategy.'
  in: query
  name: ProductionNativeFlag
  parameter: _is_native
  sources:
  - openapi/clerk-frontend-api-openapi.yml
  type: apiKey
- description: HTTP Basic Authentication using Client ID as username and Client Secret as password.
  name: ClientCredentials
  scheme: basic
  sources:
  - openapi/clerk-frontend-api-openapi.yml
  type: http
slug: clerk-com-authentication
source_filename: clerk-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clerk-backend-api-openapi.yml, openapi/clerk-frontend-api-openapi.yml, openapi/clerk-platform-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: sk_<environment>_<secret value>\n  description: Secret key, obtained under \"API Keys\" in the Clerk Dashboard.\n  sources:\n  - openapi/clerk-backend-api-openapi.yml\n  - openapi/clerk-frontend-api-openapi.yml\n  - openapi/clerk-platform-api-openapi.yml\n- name: ProductionBrowser\n  type: apiKey\n  in: cookie\n  parameter: __client\n  description: |-\n    The Client API token sent in the form of a browser cookie.\n\n    Used to authenticate production browser applications.\n  sources:\n  - openapi/clerk-frontend-api-openapi.yml\n- name: DevBrowser\n  type: apiKey\n  in: query\n  parameter: __dev_session\n  description: |-\n    A Dev Browser API token sent\
  \ as a query parameter.\n\n    Used to authenticate only dev instances.\n\n    To generate a dev instance API token you must first make a request to `/v1/dev_browser`\n    and copy it from the response.\n  sources:\n  - openapi/clerk-frontend-api-openapi.yml\n- name: ProductionNativeFlag\n  type: apiKey\n  in: query\n  parameter: _is_native\n  description: |-\n    If sent and the value is true, it instructs the server to parse the API token from the `Authorization` header.\n\n    It should always be set to true when using the `Authorization` header authentication strategy.\n  sources:\n  - openapi/clerk-frontend-api-openapi.yml\n- name: ClientCredentials\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Client ID as username and Client Secret as password.\n  sources:\n  - openapi/clerk-frontend-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clerk-com/refs/heads/main/authentication/clerk-com-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Authentication
- Authorization
- B2B SaaS
- CIAM
- Identity Management
- MFA
- OAuth
- OpenID Connect
- Organizations
- Passkeys
- SAML
- Security
- Sessions
- SSO
- User Management
---
