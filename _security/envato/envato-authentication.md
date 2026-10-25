---
anonymous_access: false
api_key_in: []
api_specs:
- filename: envato-market-api-openapi.yml
  format: yaml
  label: Envato Market API
  slug: envato-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envato/refs/heads/main/openapi/envato-market-api-openapi.yml
- filename: envato-search-api-openapi.yml
  format: yaml
  label: Envato Search API
  slug: envato-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envato/refs/heads/main/openapi/envato-search-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Envato Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Envato secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Envato
provider_slug: envato
scheme_count: 2
schemes:
- description: '"The Envato Market API supports the full OAuth authentication flow, so that you can allow users of your app to sign in with their Envato Account in order to access the API on their behalf." Apps are registered at https://build.envato.com/my-apps with the permissions they need.'
  flows:
  - authorizationUrl: https://api.envato.com/authorization
    flow: authorizationCode
    notes: The [REDIRECT URI] (Confirmation URL) must use https://. Token request is sent "encoded as application/x-www-form-urlencoded".
    refresh: refresh_token returned with the access token; used to request a new access token
    tokenUrl: https://api.envato.com/token
    token_lifetime: 'expires_in: 3600 ("valid for up to an hour")'
  - authorizationUrl: https://api.envato.com/authorization
    flow: implicit
    notes: '"the Envato API also supports the alternate, implicit OAuth authentication flow, if you are developing a browser-based app" (declared in the OpenAPI as the only flow).'
  name: oauth2
  scopes: 18
  scopes_ref: scopes/envato-scopes.yml
  sources:
  - openapi/envato-openapi.yml
  - https://build.envato.com/api/
  type: oauth2
- description: '"you can simply generate a personal token, and then insert it directly into the authorization header on any API requests: curl -H "Authorization: Bearer ..."". Generated at https://build.envato.com/create-token/.'
  header: Authorization
  name: personalToken
  scheme: bearer
  sources:
  - https://build.envato.com/api/
  type: http
slug: envato-authentication
source_filename: envato-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource: https://build.envato.com/api/\ndocs: https://build.envato.com/api/\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: oauth2\n  type: oauth2\n  description: >-\n    \"The Envato Market API supports the full OAuth authentication flow, so that you can allow users of\n    your app to sign in with their Envato Account in order to access the API on their behalf.\" Apps are\n    registered at https://build.envato.com/my-apps with the permissions they need.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.envato.com/authorization\n    tokenUrl: https://api.envato.com/token\n    token_lifetime: 'expires_in: 3600 (\"valid for up to an hour\")'\n    refresh: refresh_token returned with the access token; used to request a new access token\n    notes: 'The [REDIRECT URI] (Confirmation URL) must use https://. Token request is sent \"encoded as application/x-www-form-urlencoded\"\
  .'\n  - flow: implicit\n    authorizationUrl: https://api.envato.com/authorization\n    notes: '\"the Envato API also supports the alternate, implicit OAuth authentication flow, if you are developing a browser-based app\" (declared in the OpenAPI as the only flow).'\n  scopes: 18\n  scopes_ref: scopes/envato-scopes.yml\n  sources:\n  - openapi/envato-openapi.yml\n  - https://build.envato.com/api/\n- name: personalToken\n  type: http\n  scheme: bearer\n  description: >-\n    \"you can simply generate a personal token, and then insert it directly into the authorization header\n    on any API requests: curl -H \"Authorization: Bearer ...\"\". Generated at https://build.envato.com/create-token/.\n  header: Authorization\n  sources:\n  - https://build.envato.com/api/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envato/refs/heads/main/authentication/envato-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Stock Media
- Marketplace
- Themes
- Audio
- Video
- Graphics
- Subscription
- Australia
---
