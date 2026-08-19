---
api_key_in:
- header
api_specs:
- filename: lafourchette-b2b-api-openapi.yml
  format: yaml
  label: TheFork B2B API
  slug: thefork-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lafourchette/refs/heads/main/openapi/lafourchette-b2b-api-openapi.yml
- filename: lafourchette-pos-api-openapi.yml
  format: yaml
  label: TheFork POS API v1
  slug: thefork-pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lafourchette/refs/heads/main/openapi/lafourchette-pos-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lafourchette Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: LaFourchette secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: LaFourchette
provider_slug: lafourchette
scheme_count: 3
schemes:
- api: TheFork POS API v1
  declared_in_spec: true
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/lafourchette-pos-api-openapi.yml
  type: apiKey
- api: TheFork B2B API
  audience: https://api.thefork.io
  declared_in_spec: false
  discovery: well-known/lafourchette-openid-configuration.json
  docs: https://docs.thefork.io/B2B-API/authentication
  flow: clientCredentials
  name: Auth0ClientCredentials
  notes:
  - TheFork's docs explicitly warn against requesting a new token before the previous one expires.
  presented_as: 'Authorization: Bearer <access_token>'
  provider: Auth0 (custom domain auth.thefork.io)
  sources:
  - https://docs.thefork.io/B2B-API/authentication
  - https://docs.thefork.io/preliminary-steps
  - https://auth.thefork.io/.well-known/openid-configuration
  token_ttl_seconds: 8600
  token_type: Bearer
  token_url: https://auth.thefork.io/oauth/token
  type: oauth2
- api: TheFork POS API v1 (calls TheFork makes TO the POS)
  declared_in_spec: false
  direction: inbound-to-partner
  docs: https://docs.thefork.io/preliminary-steps
  name: PosOutboundBearer
  note: The POS vendor generates a secret (oauthClientSecret) and registers it with TheFork; TheFork then presents it as a bearer token, plus a CustomerId header carrying the restaurant UUID, on every call it makes to the POS receiptOpeningUrl and oauthTokenUrl.
  scheme: bearer
  sources:
  - https://docs.thefork.io/preliminary-steps
  - https://docs.thefork.io/POS-API/goto-production
  type: http
slug: lafourchette-authentication
source_filename: lafourchette-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: openapi/lafourchette-pos-api-openapi.yml\ndocs: https://docs.thefork.io/preliminary-steps\nnote: >-\n  Two APIs, two different auth models, and they are documented in different places. The POS API v1\n  declares its scheme in the contract itself (apiKey, header X-Api-Key). The B2B API does NOT declare\n  any securityScheme in the operation objects TheFork publishes — its authentication exists only in\n  prose on the docs pages, which is a real gap in the machine-readable contract and is recorded here\n  rather than patched into the spec. Credentials for both are issued by TheFork's integrations team\n  (integrations@thefork.com); there is no self-serve key issuance.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  self_serve: false\n  credential_issuance: manual, by TheFork integrations team (integrations@thefork.com)\nschemes:\n- name: ApiKeyAuth\n  api: TheFork\
  \ POS API v1\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  declared_in_spec: true\n  sources:\n  - openapi/lafourchette-pos-api-openapi.yml\n- name: Auth0ClientCredentials\n  api: TheFork B2B API\n  type: oauth2\n  flow: clientCredentials\n  declared_in_spec: false\n  token_url: https://auth.thefork.io/oauth/token\n  audience: https://api.thefork.io\n  token_type: Bearer\n  token_ttl_seconds: 8600\n  presented_as: 'Authorization: Bearer <access_token>'\n  provider: Auth0 (custom domain auth.thefork.io)\n  discovery: well-known/lafourchette-openid-configuration.json\n  docs: https://docs.thefork.io/B2B-API/authentication\n  sources:\n  - https://docs.thefork.io/B2B-API/authentication\n  - https://docs.thefork.io/preliminary-steps\n  - https://auth.thefork.io/.well-known/openid-configuration\n  notes:\n  - TheFork's docs explicitly warn against requesting a new token before the previous one expires.\n- name: PosOutboundBearer\n  api: TheFork POS API v1 (calls TheFork makes TO\
  \ the POS)\n  direction: inbound-to-partner\n  type: http\n  scheme: bearer\n  declared_in_spec: false\n  note: >-\n    The POS vendor generates a secret (oauthClientSecret) and registers it with TheFork; TheFork then\n    presents it as a bearer token, plus a CustomerId header carrying the restaurant UUID, on every\n    call it makes to the POS receiptOpeningUrl and oauthTokenUrl.\n  docs: https://docs.thefork.io/preliminary-steps\n  sources:\n  - https://docs.thefork.io/preliminary-steps\n  - https://docs.thefork.io/POS-API/goto-production\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lafourchette/refs/heads/main/authentication/lafourchette-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Company
- Consumer
- Restaurants
- Reservations
- Booking
- Hospitality
- Point of Sale
- Reviews
- Marketplace
- Travel and Dining
- Webhooks
- France
---
