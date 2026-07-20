---
api_key_in:
- header
api_specs:
- filename: appdirect-companies-openapi-original.yml
  format: yaml
  label: AppDirect Companies / Marketplace API
  slug: appdirect-companies-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdirect/refs/heads/main/openapi/appdirect-companies-openapi-original.yml
- filename: appdirect-devsai-openapi-original.json
  format: json
  label: AppDirect Devs.ai API
  slug: appdirect-devsai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdirect/refs/heads/main/openapi/appdirect-devsai-openapi-original.json
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Appdirect Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- password
- clientCredentials
overview: AppDirect secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, password, and clientCredentials flow(s).
provider_name: AppDirect
provider_slug: appdirect
scheme_count: 2
schemes:
- api: Companies / Marketplace REST + GraphQL API
  flows:
  - docs: https://developer.appdirect.com/user-guides/api-usage/api-auth/grant-type/credentials
    flow: clientCredentials
    tokenUrl: https://{marketplaceURL}/oauth2/token
  - docs: https://developer.appdirect.com/user-guides/api-usage/api-auth/grant-type/password
    flow: password
    tokenUrl: https://{marketplaceURL}/oauth2/token
  - authorizationUrl: https://{marketplaceURL}/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://{marketplaceURL}/oauth2/token
  - authorizationUrl: https://{marketplaceURL}/oauth2/authorize
    flow: implicit
  name: OAuth2
  note: 'The AppDirect marketplace REST and GraphQL APIs use OAuth 2.0 (OAuth 1.0 was deprecated 2020-12-01). Token endpoints are marketplace-scoped: https://{marketplaceURL}/oauth2/token and /oauth2/authorize. Grant type determines access level (user vs system); scopes correspond to AppDirect roles.'
  source: https://developer.appdirect.com/user-guides/api-usage/api-auth
  type: oauth2
- api: Devs.ai API
  description: 'Devs.ai API uses a bearer token in the Authorization header (format: Bearer {token}). Legacy header X-Authorization is also supported for backwards compatibility.'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/appdirect-devsai-openapi-original.json
  type: apiKey
slug: appdirect-authentication
source_filename: appdirect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/appdirect-devsai-openapi-original.json + https://developer.appdirect.com/user-guides/api-usage/api-auth\ndocs: https://developer.appdirect.com/user-guides/api-usage/api-auth\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - password\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  api: Companies / Marketplace REST + GraphQL API\n  source: https://developer.appdirect.com/user-guides/api-usage/api-auth\n  note: >-\n    The AppDirect marketplace REST and GraphQL APIs use OAuth 2.0 (OAuth 1.0 was\n    deprecated 2020-12-01). Token endpoints are marketplace-scoped:\n    https://{marketplaceURL}/oauth2/token and /oauth2/authorize. Grant type\n    determines access level (user vs system); scopes correspond to AppDirect roles.\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{marketplaceURL}/oauth2/token\n    docs:\
  \ https://developer.appdirect.com/user-guides/api-usage/api-auth/grant-type/credentials\n  - flow: password\n    tokenUrl: https://{marketplaceURL}/oauth2/token\n    docs: https://developer.appdirect.com/user-guides/api-usage/api-auth/grant-type/password\n  - flow: authorizationCode\n    authorizationUrl: https://{marketplaceURL}/oauth2/authorize\n    tokenUrl: https://{marketplaceURL}/oauth2/token\n  - flow: implicit\n    authorizationUrl: https://{marketplaceURL}/oauth2/authorize\n- name: ApiKeyAuth\n  type: apiKey\n  api: Devs.ai API\n  in: header\n  parameter: Authorization\n  description: >-\n    Devs.ai API uses a bearer token in the Authorization header (format: Bearer {token}).\n    Legacy header X-Authorization is also supported for backwards compatibility.\n  sources:\n  - openapi/appdirect-devsai-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appdirect/refs/heads/main/authentication/appdirect-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Commerce
- Subscription Commerce
- Marketplace
- Billing
- Reseller
- Cloud Distribution
- Webhooks
- OAuth
---
