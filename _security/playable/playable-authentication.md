---
api_key_in: []
api_specs:
- filename: playable-campaigns-api-openapi.yml
  format: yaml
  label: Playable Campaigns API
  slug: playable-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playable/refs/heads/main/openapi/playable-campaigns-api-openapi.yml
- filename: playable-media-api-openapi.yml
  format: yaml
  label: Playable Media API
  slug: playable-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playable/refs/heads/main/openapi/playable-media-api-openapi.yml
- filename: playable-oauth-api-openapi.yml
  format: yaml
  label: Playable OAUTH API
  slug: playable-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playable/refs/heads/main/openapi/playable-oauth-api-openapi.yml
- filename: playable-user-api-openapi.yml
  format: yaml
  label: Playable User API
  slug: playable-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playable/refs/heads/main/openapi/playable-user-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Playable Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Playable secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Playable
provider_slug: playable
scheme_count: 1
schemes:
- applied: Document-level security requirement lists all 37 scopes; each operation additionally narrows to the single scope it needs, so per-operation least privilege is expressible.
  flows:
  - absolute_token_url: https://api.playable.com/oauth/token
    flow: clientCredentials
    scopes: 37
    tokenUrl: /oauth/token
  name: clientCredentials
  naming_note: The scheme is named after the grant type ("clientCredentials") rather than given an identity name. Cosmetic, but it means a generated client's scheme identifier reads as a grant.
  sources:
  - openapi/playable-api-openapi.yml
  type: oauth2
slug: playable-authentication
source_filename: playable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: openapi/playable-api-openapi.yml\ndocs: https://help.playable.com/en/articles/10384051-developer\nreference: https://api.playable.com/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\n  scope_count: 37\nschemes:\n- name: clientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n    absolute_token_url: https://api.playable.com/oauth/token\n    scopes: 37\n  sources:\n  - openapi/playable-api-openapi.yml\n  applied: >-\n    Document-level security requirement lists all 37 scopes; each operation additionally narrows to\n    the single scope it needs, so per-operation least privilege is expressible.\n  naming_note: >-\n    The scheme is named after the grant type (\"clientCredentials\") rather than given an identity\n    name. Cosmetic, but it means a generated client's scheme identifier reads as a grant.\nrequest_contract:\n  header: 'Authorization:\
  \ Bearer {{ACCESS_TOKEN}}'\n  required_accept: application/json\n  accept_note: Only application/json is supported for the response type.\ncredentials:\n  self_serve: false\n  where: 'In-platform: Global settings / Developer apps'\n  docs: https://help.playable.com/en/articles/10384051-developer\n  entitlement: >-\n    API integrations are listed only on the Premium tier of the published pricing page; Essentials\n    and Core do not include API access. A prospective integrator cannot obtain credentials without a\n    Premium contract, and there is no public signup or free developer key.\n  rotation_policy: not published\n  key_prefixes: none\ntoken:\n  grant: client_credentials\n  refresh: false\n  lifetime: not published\n  expiry_signal: >-\n    The only documented failure mode is HTTP 401 with {\"message\": \"Unauthenticated.\"}, described in\n    the spec as \"Token has expired\". Re-issue on 401; there is no refresh token in this grant.\nmcp_surface:\n  note: >-\n    A SECOND, unrelated\
  \ authorization surface exists on the web property for the MCP endpoint —\n    OAuth 2.0 authorization_code + refresh_token with PKCE S256, scope `mcp`, issuer\n    https://playable.com. It is advertised via RFC 8414/RFC 9728 metadata and does NOT govern the\n    campaign API. See mcp/playable-mcp.yml and well-known/playable-well-known.yml.\nother_mechanisms:\n  saml_sso:\n    scope: platform user login only, not API access\n    docs: https://help.playable.com/en/articles/10384051-developer\n  webhook_outbound:\n    note: >-\n      When Playable calls a customer endpoint it can authenticate with OAuth 2.0, a bearer token, or\n      HTTP basic — see asyncapi/playable-webhooks.yml. That is Playable authenticating TO you.\nnot_present:\n- apiKey\n- http basic (inbound)\n- openIdConnect discovery\n- mutualTLS\n- request signing / HMAC\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playable/refs/heads/main/authentication/playable-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- marketing-gamification
- interactive-marketing
- campaign-management
- zero-party-data
- lead-generation
- loyalty
- martech
- Webhook
- Authentication
---
