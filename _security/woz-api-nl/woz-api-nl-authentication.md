---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: woz-api-nl-account-api-openapi.yml
  format: yaml
  label: woz-api-nl Account API
  slug: woz-api-nl-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/woz-api-nl/openapi/woz-api-nl-account-api-openapi.yml
- filename: woz-api-nl-adressen-api-openapi.yml
  format: yaml
  label: woz-api-nl Adressen API
  slug: woz-api-nl-adressen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/woz-api-nl/openapi/woz-api-nl-adressen-api-openapi.yml
- filename: woz-api-nl-lijst-api-openapi.yml
  format: yaml
  label: woz-api-nl Lijst API
  slug: woz-api-nl-lijst-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/woz-api-nl/openapi/woz-api-nl-lijst-api-openapi.yml
- filename: woz-api-nl-proef-api-openapi.yml
  format: yaml
  label: woz-api-nl Proef API
  slug: woz-api-nl-proef-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/woz-api-nl/openapi/woz-api-nl-proef-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Woz Api Nl Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: woz-api-nl secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: woz-api-nl
provider_slug: woz-api-nl
scheme_count: 2
schemes:
- description: 'Gebruik je API key via header: X-Api-Key: {key} of Authorization: ApiKey {key}'
  in: header
  name: ApiKey
  parameter: X-Api-Key
  sources:
  - openapi/woz-api-nl-openapi.json
  type: apiKey
- description: 'OAuth-koppeling voor softwareleveranciers: authorization code met PKCE. Je klant koppelt zijn eigen Wozapi-account; credits gaan van diens saldo af.'
  flows:
  - authorizationUrl: https://woz-api.nl/connect/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://woz-api.nl/connect/token
  name: OAuth2
  sources:
  - openapi/woz-api-nl-openapi.json
  type: oauth2
slug: woz-api-nl-authentication
source_filename: woz-api-nl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/woz-api-nl-openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: 'Gebruik je API key via header: X-Api-Key: {key} of Authorization: ApiKey {key}'\n  sources:\n  - openapi/woz-api-nl-openapi.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://woz-api.nl/connect/authorize\n    tokenUrl: https://woz-api.nl/connect/token\n    scopes: 2\n  description: 'OAuth-koppeling voor softwareleveranciers: authorization code met PKCE. Je klant\n    koppelt zijn eigen Wozapi-account; credits gaan van diens saldo af.'\n  sources:\n  - openapi/woz-api-nl-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/woz-api-nl/authentication/woz-api-nl-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Real Estate
- Netherlands
- Property Valuation
- WOZ
---
