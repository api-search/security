---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: capgo-app-api-keys-api-openapi.yml
  format: yaml
  label: Capgo API Keys API
  slug: capgo-app-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-api-keys-api-openapi.yml
- filename: capgo-app-apps-api-openapi.yml
  format: yaml
  label: Capgo Apps API
  slug: capgo-app-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-apps-api-openapi.yml
- filename: capgo-app-bundles-api-openapi.yml
  format: yaml
  label: Capgo Bundles API
  slug: capgo-app-bundles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-bundles-api-openapi.yml
- filename: capgo-app-channels-api-openapi.yml
  format: yaml
  label: Capgo Channels API
  slug: capgo-app-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-channels-api-openapi.yml
- filename: capgo-app-devices-api-openapi.yml
  format: yaml
  label: Capgo Devices API
  slug: capgo-app-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-devices-api-openapi.yml
- filename: capgo-app-members-api-openapi.yml
  format: yaml
  label: Capgo Members API
  slug: capgo-app-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-members-api-openapi.yml
- filename: capgo-app-organizations-api-openapi.yml
  format: yaml
  label: Capgo Organizations API
  slug: capgo-app-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-organizations-api-openapi.yml
- filename: capgo-app-statistics-api-openapi.yml
  format: yaml
  label: Capgo Statistics API
  slug: capgo-app-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-statistics-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Capgo App Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Capgo secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Capgo
provider_slug: capgo-app
scheme_count: 4
schemes:
- description: Send the raw Capgo API key in the `x-api-key` header. Generate or rotate keys at https://console.capgo.app/settings/organization/api-keys.
  in: header
  name: CapgoApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/capgo-app-openapi.json
  type: apiKey
- bearerFormat: Capgo API key
  description: 'Send a Capgo API key, or an access token from the Capgo OAuth flow, as `Authorization: Bearer <key>`.'
  name: CapgoBearerAuth
  scheme: bearer
  sources:
  - openapi/capgo-app-openapi.json
  type: http
- description: 'OAuth 2.0 authorization code flow with PKCE (S256) and dynamic client registration (https://api.capgo.app/mcp/oauth/register). Issuer: https://capgo.app. The access token is a Capgo API key limited to the organizations the user selects on the consent screen; send it as a Bearer token.'
  flows:
  - authorizationUrl: https://api.capgo.app/mcp/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.capgo.app/mcp/oauth/token
  name: CapgoOAuth
  sources:
  - openapi/capgo-app-openapi.json
  type: oauth2
- description: Legacy raw API key in the `authorization` header without a Bearer prefix. Prefer `x-api-key`.
  in: header
  name: CapgoLegacyAuthorization
  parameter: authorization
  sources:
  - openapi/capgo-app-openapi.json
  type: apiKey
slug: capgo-app-authentication
source_filename: capgo-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/capgo-app-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: CapgoApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Send the raw Capgo API key in the `x-api-key` header. Generate or rotate keys\n    at https://console.capgo.app/settings/organization/api-keys.\n  sources:\n  - openapi/capgo-app-openapi.json\n- name: CapgoBearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Capgo API key\n  description: 'Send a Capgo API key, or an access token from the Capgo OAuth flow, as `Authorization:\n    Bearer <key>`.'\n  sources:\n  - openapi/capgo-app-openapi.json\n- name: CapgoOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.capgo.app/mcp/oauth/authorize\n    tokenUrl: https://api.capgo.app/mcp/oauth/token\n    scopes: 1\n  description: 'OAuth\
  \ 2.0 authorization code flow with PKCE (S256) and dynamic client registration\n    (https://api.capgo.app/mcp/oauth/register). Issuer: https://capgo.app. The access token\n    is a Capgo API key limited to the organizations the user selects on the consent screen;\n    send it as a Bearer token.'\n  sources:\n  - openapi/capgo-app-openapi.json\n- name: CapgoLegacyAuthorization\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: Legacy raw API key in the `authorization` header without a Bearer prefix. Prefer\n    `x-api-key`.\n  sources:\n  - openapi/capgo-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/capgo-app/authentication/capgo-app-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Company
- Artificial Intelligence
- Mobile
- Development
- Capacitor
---
