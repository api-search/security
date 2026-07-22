---
api_key_in:
- query
api_specs:
- filename: nationbuilder-v2-openapi-original.yml
  format: yaml
  label: NationBuilder v2 API
  slug: nationbuilder-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nationbuilder/refs/heads/main/openapi/nationbuilder-v2-openapi-original.yml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nationbuilder Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: NationBuilder secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: NationBuilder
provider_slug: nationbuilder
scheme_count: 2
schemes:
- access_token_ttl_hours: 24
  applies_to: v2
  authorizationUrl: https://{nation-slug}.nationbuilder.com/oauth/authorize
  authorization_code_ttl_minutes: 10
  docs: https://support.nationbuilder.com/en/articles/9903805-api-authentication-guide
  flow: authorizationCode
  name: OAuth2AuthorizationCode
  pkce: optional
  refresh: true
  refresh_grant: refresh_token
  registration: Settings > Developer (register an application to obtain client_id / client_secret)
  tokenUrl: https://{nation-slug}.nationbuilder.com/oauth/token
  token_type: bearer
  type: oauth2
- also_accepts:
  - __token
  applies_to: v1
  docs: https://support.nationbuilder.com/en/articles/9559128-generating-api-tokens
  in: query
  name: LegacyApiToken
  note: Legacy v1 API token minted per nation. Test tokens available at https://nationbuilder.com/test_tokens. Migration to v2 OAuth is documented in the Access Token Migration Guide.
  parameter: access_token
  type: apiKey
slug: nationbuilder-authentication
source_filename: nationbuilder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://support.nationbuilder.com/en/articles/9903805-api-authentication-guide\ndocs: https://support.nationbuilder.com/en/articles/9903805-api-authentication-guide\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [query]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    NationBuilder is multi-tenant: every nation is reached at its own\n    {nation-slug}.nationbuilder.com host. The current v2 API authenticates with\n    OAuth 2.0 authorization-code (PKCE optional). The legacy v1 API accepts a\n    per-nation API token.\nschemes:\n  - name: OAuth2AuthorizationCode\n    type: oauth2\n    applies_to: v2\n    flow: authorizationCode\n    pkce: optional\n    authorizationUrl: https://{nation-slug}.nationbuilder.com/oauth/authorize\n    tokenUrl: https://{nation-slug}.nationbuilder.com/oauth/token\n    token_type: bearer\n    access_token_ttl_hours: 24\n    refresh: true\n    refresh_grant: refresh_token\n    authorization_code_ttl_minutes:\
  \ 10\n    registration: Settings > Developer (register an application to obtain client_id / client_secret)\n    docs: https://support.nationbuilder.com/en/articles/9903805-api-authentication-guide\n  - name: LegacyApiToken\n    type: apiKey\n    applies_to: v1\n    in: query\n    parameter: access_token\n    also_accepts: [__token]\n    note: >-\n      Legacy v1 API token minted per nation. Test tokens available at\n      https://nationbuilder.com/test_tokens. Migration to v2 OAuth is documented\n      in the Access Token Migration Guide.\n    docs: https://support.nationbuilder.com/en/articles/9559128-generating-api-tokens\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nationbuilder/refs/heads/main/authentication/nationbuilder-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Community Organizing
- CRM
- Political
- Nonprofit
- Fundraising
- Advocacy
- Website Builder
- Events
- Email
- JSON:API
---
