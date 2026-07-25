---
api_key_in: []
api_specs:
- filename: beyond-accounts-api-openapi.yml
  format: yaml
  label: Beyond Accounts API
  slug: beyond-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond/refs/heads/main/openapi/beyond-accounts-api-openapi.yml
- filename: beyond-compsets-api-openapi.yml
  format: yaml
  label: Beyond Compsets API
  slug: beyond-compsets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond/refs/heads/main/openapi/beyond-compsets-api-openapi.yml
- filename: beyond-customizations-api-openapi.yml
  format: yaml
  label: Beyond Customizations API
  slug: beyond-customizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond/refs/heads/main/openapi/beyond-customizations-api-openapi.yml
- filename: beyond-insights-api-openapi.yml
  format: yaml
  label: Beyond Insights API
  slug: beyond-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond/refs/heads/main/openapi/beyond-insights-api-openapi.yml
- filename: beyond-listings-api-openapi.yml
  format: yaml
  label: Beyond Listings API
  slug: beyond-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond/refs/heads/main/openapi/beyond-listings-api-openapi.yml
- filename: beyond-oauth2-api-openapi.yml
  format: yaml
  label: Beyond OAuth2 API
  slug: beyond-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond/refs/heads/main/openapi/beyond-oauth2-api-openapi.yml
- filename: beyond-users-api-openapi.yml
  format: yaml
  label: Beyond Users API
  slug: beyond-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond/refs/heads/main/openapi/beyond-users-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Beyond Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Beyond secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Beyond
provider_slug: beyond
scheme_count: 2
schemes:
- description: Use OAuth2 client credentials to mint an application token, or add `user_id` and optional `credential_id` in the Authorize dialog to request a user- or credential-scoped token.
  flows:
  - flow: clientCredentials
    scopes: 9
    tokenUrl: /o/token/
  name: oauth2
  sources:
  - openapi/beyond-openapi-original.yml
  type: oauth2
- bearerFormat: PersonalAccessToken
  description: Paste a `bpat_...` personal access token. PATs use the same Bearer header as OAuth2 tokens and must still include the runtime-required scopes for each endpoint, even though OpenAPI cannot encode scopes for non-OAuth bearer schemes.
  name: personalAccessToken
  scheme: bearer
  sources:
  - openapi/beyond-openapi-original.yml
  type: http
slug: beyond-authentication
source_filename: beyond-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/beyond-openapi-original.yml\ndocs: https://developers.beyondpricing.com/getting-started/authentication/\nstandards:\n- RFC 9700 (OAuth 2.0 Security Best Current Practice)\n- RFC 8414 (OAuth 2.0 Authorization Server Metadata)\n- RFC 7591 (Dynamic Client Registration)\nnotes: >-\n  Bearer-protected API. Partners use OAuth2 client-credentials to mint app tokens and may\n  scope tokens to a user via user_id / credential_id. Individual users paste a personal\n  access token prefixed `bpat_...` in the same Bearer header. The authorization-server\n  metadata (well-known/beyond-oauth-authorization-server.json) additionally advertises\n  authorization_code, device_code and refresh_token grants with PKCE S256; the MCP server\n  (neyoba:ask scope) uses the authorization_code + PKCE flow with dynamic client registration.\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n\
  \  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /o/token/\n    scopes: 9\n  description: Use OAuth2 client credentials to mint an application token, or add `user_id`\n    and optional `credential_id` in the Authorize dialog to request a user- or credential-scoped\n    token.\n  sources:\n  - openapi/beyond-openapi-original.yml\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: PersonalAccessToken\n  description: Paste a `bpat_...` personal access token. PATs use the same Bearer header as\n    OAuth2 tokens and must still include the runtime-required scopes for each endpoint, even\n    though OpenAPI cannot encode scopes for non-OAuth bearer schemes.\n  sources:\n  - openapi/beyond-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyond/refs/heads/main/authentication/beyond-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Consumer
- Travel
- Hospitality
- Short-Term Rentals
- Vacation Rentals
- Revenue Management
- Dynamic Pricing
- Pricing
- Real Estate
- Market Intelligence
- API
---
