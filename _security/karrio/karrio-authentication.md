---
api_key_in:
- header
api_specs:
- filename: karrio-addresses-api-openapi.yml
  format: yaml
  label: Karrio Addresses API
  slug: karrio-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-addresses-api-openapi.yml
- filename: karrio-api-api-openapi.yml
  format: yaml
  label: Karrio API
  slug: karrio-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-api-api-openapi.yml
- filename: karrio-auth-api-openapi.yml
  format: yaml
  label: Karrio Auth API
  slug: karrio-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-auth-api-openapi.yml
- filename: karrio-batches-api-openapi.yml
  format: yaml
  label: Karrio Batches API
  slug: karrio-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-batches-api-openapi.yml
- filename: karrio-carriers-api-openapi.yml
  format: yaml
  label: Karrio Carriers API
  slug: karrio-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-carriers-api-openapi.yml
- filename: karrio-connections-api-openapi.yml
  format: yaml
  label: Karrio Connections API
  slug: karrio-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-connections-api-openapi.yml
- filename: karrio-documents-api-openapi.yml
  format: yaml
  label: Karrio Documents API
  slug: karrio-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-documents-api-openapi.yml
- filename: karrio-manifests-api-openapi.yml
  format: yaml
  label: Karrio Manifests API
  slug: karrio-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-manifests-api-openapi.yml
- filename: karrio-orders-api-openapi.yml
  format: yaml
  label: Karrio Orders API
  slug: karrio-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-orders-api-openapi.yml
- filename: karrio-parcels-api-openapi.yml
  format: yaml
  label: Karrio Parcels API
  slug: karrio-parcels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-parcels-api-openapi.yml
- filename: karrio-pickups-api-openapi.yml
  format: yaml
  label: Karrio Pickups API
  slug: karrio-pickups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-pickups-api-openapi.yml
- filename: karrio-products-api-openapi.yml
  format: yaml
  label: Karrio Products API
  slug: karrio-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-products-api-openapi.yml
- filename: karrio-proxy-api-openapi.yml
  format: yaml
  label: Karrio Proxy API
  slug: karrio-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-proxy-api-openapi.yml
- filename: karrio-shipments-api-openapi.yml
  format: yaml
  label: Karrio Shipments API
  slug: karrio-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-shipments-api-openapi.yml
- filename: karrio-trackers-api-openapi.yml
  format: yaml
  label: Karrio Trackers API
  slug: karrio-trackers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-trackers-api-openapi.yml
- filename: karrio-webhooks-api-openapi.yml
  format: yaml
  label: Karrio Webhooks API
  slug: karrio-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: 'Karrio accepts four credential types, and the one most integrators reach for first is the least obvious: the API token is sent as the HTTP Basic USERNAME with an empty password. All four resolve to the same instance-scoped organization context.'
kind: authentication
layout: security
method: searched
name: Karrio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Karrio secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Karrio
provider_slug: karrio
scheme_count: 4
schemes:
- description: The primary credential. A long-lived API key issued per organization from Settings -> API Keys in the dashboard, or read from the GraphQL `token { key }` query. Carries the full privileges of the organization.
  format: 'Authorization: Token key_xxxxxxxx'
  in: header
  name: Token
  parameter: Authorization
  sources:
  - openapi/karrio-api-openapi.yml
  - https://karrio.io/docs/api-reference
  token_prefix: key_
  type: apiKey
- description: The SAME API token, supplied as the HTTP Basic username with an empty password. This is the form Karrio's own documentation leads with. The trailing colon is required — it stops curl prompting for a password.
  format: '-u key_xxxxxxxx:'
  name: TokenBasic
  quoted: '"Authentication to the API is performed via HTTP Basic Auth. Provide your API token as the basic auth username value. You do not need to provide a password."'
  scheme: basic
  sources:
  - openapi/karrio-api-openapi.yml
  - https://karrio.io/docs/api-reference
  type: http
- description: Short-lived JSON Web Token obtained from POST /api/token with username and password, refreshed at POST /api/token/refresh, verified at POST /api/token/verify. Used by the dashboard and by the GraphQL management API; also the path to issuing an API key programmatically.
  format: 'Authorization: Bearer xxx.xxx.xxx'
  in: header
  name: JWT
  operations:
  - '&&authenticate (POST /api/token)'
  - '&&refresh_token (POST /api/token/refresh)'
  - '&&verify_token (POST /api/token/verify)'
  - '&&get_verified_token (POST /api/token/verified)'
  - '&&generate_resource_token (POST /api/tokens)'
  - '&&logout (POST /api/logout)'
  parameter: Authorization
  sources:
  - openapi/karrio-api-openapi.yml
  type: apiKey
- description: Authorization-code flow for third-party applications built on a Karrio instance (the app-store / platform surface). Scopes read, write and openid. See scopes/karrio-scopes.yml.
  flows:
  - authorizationUrl: /oauth/authorize/
    flow: authorizationCode
    scopes: 3
    tokenUrl: /oauth/token/
  name: OAuth2
  sources:
  - openapi/karrio-api-openapi.yml
  type: oauth2
slug: karrio-authentication
source_filename: karrio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  openapi/karrio-api-openapi.yml (Karrio API 2026.1.32) securitySchemes, upgraded with the\n  Authentication section of the API reference at https://karrio.io/docs/api-reference and\n  the token flow documented at https://karrio.io/docs/developing/api-development.\ndocs: https://karrio.io/docs/api-reference\nprovider: Karrio\nproviderId: karrio\ndescription: >-\n  Karrio accepts four credential types, and the one most integrators reach for first is\n  the least obvious: the API token is sent as the HTTP Basic USERNAME with an empty\n  password. All four resolve to the same instance-scoped organization context.\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  primary: Token\n  transport_requirement: HTTPS. \"All API requests must be made over HTTPS. API requests without authentication will also fail.\"\nschemes:\n- name: Token\n  type: apiKey\n  in:\
  \ header\n  parameter: Authorization\n  format: 'Authorization: Token key_xxxxxxxx'\n  description: >-\n    The primary credential. A long-lived API key issued per organization from Settings ->\n    API Keys in the dashboard, or read from the GraphQL `token { key }` query. Carries\n    the full privileges of the organization.\n  token_prefix: key_\n  sources:\n  - openapi/karrio-api-openapi.yml\n  - https://karrio.io/docs/api-reference\n- name: TokenBasic\n  type: http\n  scheme: basic\n  format: '-u key_xxxxxxxx:'\n  description: >-\n    The SAME API token, supplied as the HTTP Basic username with an empty password. This\n    is the form Karrio's own documentation leads with. The trailing colon is required —\n    it stops curl prompting for a password.\n  quoted: >-\n    \"Authentication to the API is performed via HTTP Basic Auth. Provide your API token\n    as the basic auth username value. You do not need to provide a password.\"\n  sources:\n  - openapi/karrio-api-openapi.yml\n  -\
  \ https://karrio.io/docs/api-reference\n- name: JWT\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Bearer xxx.xxx.xxx'\n  description: >-\n    Short-lived JSON Web Token obtained from POST /api/token with username and password,\n    refreshed at POST /api/token/refresh, verified at POST /api/token/verify. Used by the\n    dashboard and by the GraphQL management API; also the path to issuing an API key\n    programmatically.\n  operations:\n  - '&&authenticate (POST /api/token)'\n  - '&&refresh_token (POST /api/token/refresh)'\n  - '&&verify_token (POST /api/token/verify)'\n  - '&&get_verified_token (POST /api/token/verified)'\n  - '&&generate_resource_token (POST /api/tokens)'\n  - '&&logout (POST /api/logout)'\n  sources:\n  - openapi/karrio-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize/\n    tokenUrl: /oauth/token/\n    scopes: 3\n  description: >-\n    Authorization-code\
  \ flow for third-party applications built on a Karrio instance\n    (the app-store / platform surface). Scopes read, write and openid. See\n    scopes/karrio-scopes.yml.\n  sources:\n  - openapi/karrio-api-openapi.yml\nmodes:\n  test_and_live: true\n  selected_by: the credential\n  note: >-\n    Each API key is issued as either test or live. Mode is a property of the credential,\n    not of the URL — there is no separate sandbox host. GraphQL calls can also carry\n    `x-test-mode: true`. See sandbox/karrio-sandbox.yml.\ngaps:\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server is served on any host (probed 2026-08-27, all 404 or 503), so the OAuth2 and openid surfaces are not discoverable.\n- Key rotation, expiry and revocation policy is not published.\n- No published distinction between the test-key and live-key string format; both are documented as `key_`.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/authentication/karrio-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Shipping
- Logistics
- Label Generation
- Package Tracking
- Carriers
- Fulfillment
- Open Source
- Multi-Carrier
- Rating
- Webhooks
---
