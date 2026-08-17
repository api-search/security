---
api_key_in: []
api_specs:
- filename: drip-accounts-api-openapi.yml
  format: yaml
  label: Drip Accounts API
  slug: drip-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-accounts-api-openapi.yml
- filename: drip-broadcasts-api-openapi.yml
  format: yaml
  label: Drip Broadcasts API
  slug: drip-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-broadcasts-api-openapi.yml
- filename: drip-campaigns-api-openapi.yml
  format: yaml
  label: Drip Campaigns API
  slug: drip-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-campaigns-api-openapi.yml
- filename: drip-conversions-api-openapi.yml
  format: yaml
  label: Drip Conversions API
  slug: drip-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-conversions-api-openapi.yml
- filename: drip-custom-fields-api-openapi.yml
  format: yaml
  label: Drip Custom Fields API
  slug: drip-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-custom-fields-api-openapi.yml
- filename: drip-events-api-openapi.yml
  format: yaml
  label: Drip Events API
  slug: drip-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-events-api-openapi.yml
- filename: drip-forms-api-openapi.yml
  format: yaml
  label: Drip Forms API
  slug: drip-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-forms-api-openapi.yml
- filename: drip-orders-api-openapi.yml
  format: yaml
  label: Drip Orders API
  slug: drip-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-orders-api-openapi.yml
- filename: drip-shopper-activity-api-openapi.yml
  format: yaml
  label: Drip Shopper Activity API
  slug: drip-shopper-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-shopper-activity-api-openapi.yml
- filename: drip-subscribers-api-openapi.yml
  format: yaml
  label: Drip Subscribers API
  slug: drip-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-subscribers-api-openapi.yml
auth_types:
- http
- oauth2
description: Drip authenticates the REST API two ways. Private integrations use the account's personal API token as the username half of HTTP Basic with an empty password (note the trailing colon). Public integrations use OAuth 2.0 authorization code, with the resulting bearer token in the Authorization header. Drip additionally asks every caller to send an identifying User-Agent of the form `Your App Name (www.yourapp.com)`, and the API requires a client that supports SNI.
kind: authentication
layout: security
method: searched
name: Drip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Drip secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Drip
provider_slug: drip
scheme_count: 3
schemes:
- description: Personal API Token as the Basic username with an empty password (`-u 'YOUR_API_KEY:'`). Intended for private, single-account integrations. Token is found in the Drip account settings.
  docs: https://developer.drip.com/#authentication
  name: basicAuth
  scheme: basic
  sources:
  - openapi/drip-openapi.yml
  - https://developer.drip.com/#authentication
  type: http
- bearerFormat: OAuth2 access token
  description: '`Authorization: Bearer <access_token>` using a token issued by the Drip OAuth 2.0 authorization server. Intended for public integrations acting on behalf of other people''s Drip accounts.'
  docs: https://developer.drip.com/#oauth
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/drip-openapi.yml
  - https://developer.drip.com/#oauth
  type: http
- authorizationUrl: https://www.getdrip.com/oauth/authorize
  description: Authorization code flow. Applications are registered with Drip to obtain a client id and secret and must supply a valid callback URL before they can be activated. The verification code expires in 10 minutes. Drip's docs state access tokens do not expire, though the authorization server metadata advertises refresh_token support.
  detail: scopes/drip-scopes.yml
  docs: https://developer.drip.com/#oauth
  dynamic_client_registration: true
  flow: authorizationCode
  name: oauth2
  pkce: S256
  registrationUrl: https://api.getdrip.com/oauth/register
  scopes:
    public: Default scope returned in the token response.
    write: Mutating access across the account.
  sources:
  - https://developer.drip.com/#oauth
  - well-known/drip-oauth-authorization-server.json
  tokenUrl: https://www.getdrip.com/oauth/token
  type: oauth2
slug: drip-authentication
source_filename: drip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://developer.drip.com/#authentication and\n  https://developer.drip.com/#oauth (read 2026-08-13), plus\n  https://api.getdrip.com/.well-known/oauth-authorization-server (HTTP 200).\n  Upgraded from the 2026-07-11 derived profile, which read only the two HTTP\n  schemes declared in openapi/drip-openapi.yml.\ndocs: https://developer.drip.com/#authentication\ndescription: >-\n  Drip authenticates the REST API two ways. Private integrations use the\n  account's personal API token as the username half of HTTP Basic with an empty\n  password (note the trailing colon). Public integrations use OAuth 2.0\n  authorization code, with the resulting bearer token in the Authorization\n  header. Drip additionally asks every caller to send an identifying User-Agent\n  of the form `Your App Name (www.yourapp.com)`, and the API requires a client\n  that supports SNI.\nsummary:\n  types:\n    - http\n    - oauth2\nschemes:\n  - name:\
  \ basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      Personal API Token as the Basic username with an empty password\n      (`-u 'YOUR_API_KEY:'`). Intended for private, single-account\n      integrations. Token is found in the Drip account settings.\n    docs: https://developer.drip.com/#authentication\n    sources:\n      - openapi/drip-openapi.yml\n      - https://developer.drip.com/#authentication\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: OAuth2 access token\n    description: >-\n      `Authorization: Bearer <access_token>` using a token issued by the Drip\n      OAuth 2.0 authorization server. Intended for public integrations acting\n      on behalf of other people's Drip accounts.\n    docs: https://developer.drip.com/#oauth\n    sources:\n      - openapi/drip-openapi.yml\n      - https://developer.drip.com/#oauth\n  - name: oauth2\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://www.getdrip.com/oauth/authorize\n\
  \    tokenUrl: https://www.getdrip.com/oauth/token\n    registrationUrl: https://api.getdrip.com/oauth/register\n    scopes:\n      public: Default scope returned in the token response.\n      write: Mutating access across the account.\n    pkce: S256\n    dynamic_client_registration: true\n    description: >-\n      Authorization code flow. Applications are registered with Drip to obtain\n      a client id and secret and must supply a valid callback URL before they\n      can be activated. The verification code expires in 10 minutes. Drip's\n      docs state access tokens do not expire, though the authorization server\n      metadata advertises refresh_token support.\n    docs: https://developer.drip.com/#oauth\n    detail: scopes/drip-scopes.yml\n    sources:\n      - https://developer.drip.com/#oauth\n      - well-known/drip-oauth-authorization-server.json\nconventions:\n  required_headers:\n    - name: User-Agent\n      required: recommended\n      format: Your App Name (www.yourapp.com)\n\
  \      note: Present in every curl example in the reference.\n    - name: Content-Type\n      required: true\n      value: application/json\n      note: >-\n        Parameters must be serialized as JSON in the request body — not in the\n        query string and not as form parameters.\n  transport: HTTPS only, SNI required\n  unauthenticated_response: 401 Unauthorized with an errors[] envelope\n  insufficient_permissions_response: 403 Forbidden, code authorization_error\nmcp:\n  note: >-\n    The MCP endpoint at https://api.getdrip.com/mcp is protected by the same\n    OAuth authorization server and advertises RFC 9728 protected-resource\n    metadata. See mcp/drip-mcp.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/authentication/drip-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Email Marketing
- Marketing Automation
- Ecommerce
- Customer Engagement
- Campaigns
- Workflows
---
