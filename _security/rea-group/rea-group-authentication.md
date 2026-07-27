---
api_key_in: []
api_specs:
- filename: rea-group-oauth-openapi.yml
  format: yaml
  label: PropTrack OAuth 2.0 Token API
  slug: proptrack-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-oauth-openapi.yml
- filename: rea-group-address-openapi.yml
  format: yaml
  label: PropTrack Address API
  slug: proptrack-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-address-openapi.yml
- filename: rea-group-properties-openapi.yml
  format: yaml
  label: PropTrack Properties API
  slug: proptrack-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-properties-openapi.yml
- filename: rea-group-listings-openapi.yml
  format: yaml
  label: PropTrack Listings API
  slug: proptrack-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-listings-openapi.yml
- filename: rea-group-transactions-openapi.yml
  format: yaml
  label: PropTrack Transactions API
  slug: proptrack-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-transactions-openapi.yml
- filename: rea-group-market-openapi.yml
  format: yaml
  label: PropTrack Market API
  slug: proptrack-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-market-openapi.yml
- filename: rea-group-reports-openapi.yml
  format: yaml
  label: PropTrack Reports API
  slug: proptrack-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-reports-openapi.yml
- filename: rea-group-disclaimers-openapi.yml
  format: yaml
  label: PropTrack Disclaimers API
  slug: proptrack-disclaimers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-disclaimers-openapi.yml
- filename: rea-group-coming-soon-openapi.yml
  format: yaml
  label: PropTrack Upcoming APIs (Schools)
  slug: proptrack-upcoming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-coming-soon-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Rea Group Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: REA Group secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: REA Group
provider_slug: rea-group
scheme_count: 2
schemes:
- client_authentication: client_secret_basic
  flows:
  - flow: clientCredentials
    note: No scope surface is published. The issued JWT carries a scope claim but the developer documentation does not enumerate scope values, so scopes/ is not emitted for this provider.
    scopes: {}
    tokenUrl: https://data.proptrack.com/oauth2/token
  name: OAuth2ClientCredentials
  sources:
  - https://developer.proptrack.com.au/docs/apis/how-to-authenticate
  - openapi/rea-group-oauth-openapi.yml
  type: oauth2
- applies_to: all data.proptrack.com API operations
  bearerFormat: JWT
  name: BearerToken
  scheme: bearer
  sources:
  - https://developer.proptrack.com.au/docs/apis/how-to-authenticate
  type: http
slug: rea-group-authentication
source_filename: rea-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://developer.proptrack.com.au/docs/apis/how-to-authenticate\ndocs: https://developer.proptrack.com.au/docs/apis/how-to-authenticate\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  token_type: Bearer\n  token_format: JWT\n  token_ttl_seconds: 3600\n  notes: >-\n    PropTrack (REA Group) APIs are protected by OAuth 2.0 client credentials.\n    Partners are issued an api_key and api_secret under a commercial agreement,\n    Base64-encode them as an HTTP Basic credential on the token request, and\n    exchange them at https://data.proptrack.com/oauth2/token for a JWT access\n    token with a one hour TTL. The token is then presented as a Bearer token on\n    every subsequent call to data.proptrack.com. Credentials as form parameters\n    are explicitly NOT supported - the Authorization header is the only accepted\n    channel. Credential issuance is partner-gated; there is no self-serve\
  \ signup.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://data.proptrack.com/oauth2/token\n    scopes: {}\n    note: >-\n      No scope surface is published. The issued JWT carries a scope claim but the\n      developer documentation does not enumerate scope values, so scopes/ is not\n      emitted for this provider.\n  client_authentication: client_secret_basic\n  sources:\n  - https://developer.proptrack.com.au/docs/apis/how-to-authenticate\n  - openapi/rea-group-oauth-openapi.yml\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: all data.proptrack.com API operations\n  sources:\n  - https://developer.proptrack.com.au/docs/apis/how-to-authenticate\ntoken_request:\n  method: POST\n  url: https://data.proptrack.com/oauth2/token\n  operation: openapi/rea-group-oauth-openapi.yml#auth-token\n  headers:\n    Content-Type: application/x-www-form-urlencoded\n    Authorization: Basic\
  \ base64(api_key:api_secret)\n  body:\n    grant_type: client_credentials\n  response_fields: [access_token, token_type, expires_in]\nerrors:\n  token_validation_failed: 9012\n  token_expired: 9016\n  access_denied: 9003\n  note: >-\n    A 403 Access Denied returned as an HTML body (rather than the JSON error\n    envelope) indicates an IP-level block, not a credential failure - the docs\n    direct these to support@proptrack.com.\ngaps:\n- >-\n  The published OpenAPI documents declare no components.securitySchemes, so the\n  OAuth 2.0 model documented in prose is not machine-readable from the specs.\n  Captured here and in overlays/rea-group-security-overlay.yaml.\ncross_links:\n  conventions: conventions/rea-group-conventions.yml\n  errors: errors/rea-group-error-codes.yml\n  openapi: openapi/rea-group-oauth-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/authentication/rea-group-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Real Estate
- Property Data
- Valuations
- AVM
- Market Insights
- Listings
- Transactions
- Address Matching
- REAXML
- Partner Portal
- PropTech
- Australia
---
