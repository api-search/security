---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: makefx-app-asset-api-openapi.yml
  format: yaml
  label: makefx Asset API
  slug: makefx-app-asset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-asset-api-openapi.yml
- filename: makefx-app-auth-api-openapi.yml
  format: yaml
  label: makefx Auth API
  slug: makefx-app-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-auth-api-openapi.yml
- filename: makefx-app-link-api-openapi.yml
  format: yaml
  label: makefx Link API
  slug: makefx-app-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-link-api-openapi.yml
- filename: makefx-app-models-api-openapi.yml
  format: yaml
  label: makefx Models API
  slug: makefx-app-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-models-api-openapi.yml
- filename: makefx-app-oauth-api-openapi.yml
  format: yaml
  label: makefx OAuth API
  slug: makefx-app-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-oauth-api-openapi.yml
- filename: makefx-app-p-api-openapi.yml
  format: yaml
  label: makefx P API
  slug: makefx-app-p-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-p-api-openapi.yml
- filename: makefx-app-service-api-openapi.yml
  format: yaml
  label: makefx Service API
  slug: makefx-app-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-service-api-openapi.yml
- filename: makefx-app-space-api-openapi.yml
  format: yaml
  label: makefx Space API
  slug: makefx-app-space-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-space-api-openapi.yml
- filename: makefx-app-user-api-openapi.yml
  format: yaml
  label: makefx User API
  slug: makefx-app-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-user-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: makefx Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: makefx secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: makefx
provider_slug: makefx-app
scheme_count: 3
schemes:
- description: 'OAuth 2.1 authorization code with PKCE (S256), issued by this deployment. Register a client at the registration endpoint or present a Client ID Metadata Document, then send the person to authorize. Metadata: /.well-known/oauth-authorization-server.'
  flows:
  - authorizationUrl: https://makefx.app/api/oauth/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://makefx.app/api/oauth/token
  name: oauth2
  sources:
  - openapi/makefx-app-openapi.json
  type: oauth2
- description: The browser session set by signing in with Google. Routes that manage the account itself accept only this, never an app token.
  in: cookie
  name: session
  parameter: auth_token
  sources:
  - openapi/makefx-app-openapi.json
  type: apiKey
- description: The registration access token returned by client registration (RFC 7592). It manages that one registration and nothing else.
  name: registrationToken
  scheme: bearer
  sources:
  - openapi/makefx-app-openapi.json
  type: http
slug: makefx-app-authentication
source_filename: makefx-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/makefx-app-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://makefx.app/api/oauth/authorize\n    tokenUrl: https://makefx.app/api/oauth/token\n    scopes: 5\n  description: 'OAuth 2.1 authorization code with PKCE (S256), issued by this deployment. Register\n    a client at the registration endpoint or present a Client ID Metadata Document, then send\n    the person to authorize. Metadata: /.well-known/oauth-authorization-server.'\n  sources:\n  - openapi/makefx-app-openapi.json\n- name: session\n  type: apiKey\n  in: cookie\n  parameter: auth_token\n  description: The browser session set by signing in with Google. Routes that manage the account\n    itself accept only this, never an app token.\n  sources:\n  - openapi/makefx-app-openapi.json\n\
  - name: registrationToken\n  type: http\n  scheme: bearer\n  description: The registration access token returned by client registration (RFC 7592). It\n    manages that one registration and nothing else.\n  sources:\n  - openapi/makefx-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/makefx-app/authentication/makefx-app-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Artificial Intelligence
- Media
- Platform
- Creators
- Payments
---
