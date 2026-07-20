---
api_key_in: []
api_specs:
- filename: beyond-pricing-openapi-original.yml
  format: yaml
  label: Beyond Pricing Public API
  slug: beyond-pricing-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-pricing/refs/heads/main/openapi/beyond-pricing-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Beyond Pricing Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Beyond Pricing secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Beyond Pricing
provider_slug: beyond-pricing
scheme_count: 2
schemes:
- description: Use OAuth2 client credentials to mint an application token, or add `user_id` and optional `credential_id` in the Authorize dialog to request a user- or credential-scoped token.
  flows:
  - flow: clientCredentials
    scopes: 9
    tokenUrl: /o/token/
  name: oauth2
  sources:
  - openapi/beyond-pricing-openapi-original.yml
  type: oauth2
- bearerFormat: PersonalAccessToken
  description: Paste a `bpat_...` personal access token. PATs use the same Bearer header as OAuth2 tokens and must still include the runtime-required scopes for each endpoint, even though OpenAPI cannot encode scopes for non-OAuth bearer schemes.
  name: personalAccessToken
  scheme: bearer
  sources:
  - openapi/beyond-pricing-openapi-original.yml
  type: http
slug: beyond-pricing-authentication
source_filename: beyond-pricing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/beyond-pricing-openapi-original.yml\ndocs: https://developers.beyondpricing.com/getting-started/authentication/\nstandards:\n- RFC 9700 (OAuth 2.0 Security Best Current Practice)\n- RFC 8414 (OAuth 2.0 Authorization Server Metadata)\nauthorization_server_metadata: https://developers.beyondpricing.com/.well-known/oauth-authorization-server\nnotes: >-\n  Partners use OAuth2 client-credentials on a confidential client; access tokens\n  expire after 1 hour and can be narrowed with user_id (user-scoped) and\n  credential_id (credential-scoped). Individual users use self-service personal\n  access tokens (bpat_ prefix) created in the Beyond dashboard, sent as\n  Authorization: Bearer. IP allowlists can be enforced per application.\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /o/token/\n    scopes:\
  \ 9\n  description: Use OAuth2 client credentials to mint an application token, or add `user_id`\n    and optional `credential_id` in the Authorize dialog to request a user- or credential-scoped\n    token.\n  sources:\n  - openapi/beyond-pricing-openapi-original.yml\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: PersonalAccessToken\n  description: Paste a `bpat_...` personal access token. PATs use the same Bearer header as\n    OAuth2 tokens and must still include the runtime-required scopes for each endpoint, even\n    though OpenAPI cannot encode scopes for non-OAuth bearer schemes.\n  sources:\n  - openapi/beyond-pricing-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyond-pricing/refs/heads/main/authentication/beyond-pricing-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Short-Term Rentals
- Vacation Rentals
- Revenue Management
- Dynamic Pricing
- Hospitality
- Property Management
- Travel
- Pricing
- JSON:API
---
