---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Jampp Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Jampp secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Jampp
provider_slug: jampp
scheme_count: 2
schemes:
- credential_issuance: https://app.jampp.com/users/credentials
  credential_note: Client ID / client secret pairs are self-issued from the Credentials section of the Silver dashboard. Jampp documents creating one key pair per integrating service so a single key can be revoked without affecting the others.
  flow: clientCredentials
  name: OAuth2ClientCredentials
  parameters:
  - grant_type (must be the exact string client_credentials)
  - client_id
  - client_secret
  request_content_type: application/x-www-form-urlencoded
  response_fields:
  - access_token
  - token_type
  - expires_in
  sources:
  - https://developers.jampp.com/docs/reporting-api/
  token_lifetime_seconds: 7200
  token_type: Bearer
  token_url: https://auth.jampp.com/v1/oauth/token
  type: oauth2
  usage: 'Authorization: Bearer {access_token} on every Reporting API request'
- advertised_only: true
  authorization_url: https://auth.jampp.com/v1/oauth/authorize
  flow: authorizationCode
  name: OAuth2AuthorizationCode
  note: Advertised in the authorization-server metadata (grant_types_supported also lists refresh_token) but not documented in the developer docs, which cover only the client-credentials flow. Recorded as advertised, not as a documented developer path.
  pkce:
  - S256
  registration_url: https://auth.jampp.com/v1/oauth/register
  sources:
  - https://auth.jampp.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  token_url: https://auth.jampp.com/v1/oauth/token
  type: oauth2
slug: jampp-authentication
source_filename: jampp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://developers.jampp.com/docs/reporting-api/\ndocs: https://developers.jampp.com/docs/reporting-api/\nprobe_source: https://auth.jampp.com/.well-known/oauth-authorization-server\nnote: >-\n  Derived by hand from the published Reporting API documentation and from the RFC 8414\n  authorization-server metadata Jampp actually serves. There is no OpenAPI to run\n  derive-authentication.py against — the only public contract is a GraphQL endpoint whose\n  introspection is auth-gated.\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [clientCredentials, authorizationCode]\n  documented_flow: clientCredentials\n  bearer_methods: [header]\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://auth.jampp.com/v1/oauth/token\n  request_content_type: application/x-www-form-urlencoded\n  parameters:\n  - grant_type (must be the exact string client_credentials)\n  - client_id\n\
  \  - client_secret\n  response_fields: [access_token, token_type, expires_in]\n  token_type: Bearer\n  token_lifetime_seconds: 7200\n  usage: 'Authorization: Bearer {access_token} on every Reporting API request'\n  credential_issuance: https://app.jampp.com/users/credentials\n  credential_note: >-\n    Client ID / client secret pairs are self-issued from the Credentials section of the\n    Silver dashboard. Jampp documents creating one key pair per integrating service so a\n    single key can be revoked without affecting the others.\n  sources: [https://developers.jampp.com/docs/reporting-api/]\n- name: OAuth2AuthorizationCode\n  type: oauth2\n  flow: authorizationCode\n  authorization_url: https://auth.jampp.com/v1/oauth/authorize\n  token_url: https://auth.jampp.com/v1/oauth/token\n  registration_url: https://auth.jampp.com/v1/oauth/register\n  pkce: [S256]\n  token_endpoint_auth_methods: [none]\n  advertised_only: true\n  note: >-\n    Advertised in the authorization-server metadata\
  \ (grant_types_supported also lists\n    refresh_token) but not documented in the developer docs, which cover only the\n    client-credentials flow. Recorded as advertised, not as a documented developer path.\n  sources: [https://auth.jampp.com/.well-known/oauth-authorization-server]\ntoken_validation:\n  jwks_uri: https://auth.jampp.com/.well-known/jwks.json\n  algorithms: [ES256]\n  curve: secp256k1\n  key_ids: [v1, v2]\nprotected_resources:\n- resource: https://api.jampp.com\n  authorization_servers: [https://auth.jampp.com]\n  bearer_methods_supported: [header]\n  source: https://api.jampp.com/.well-known/oauth-protected-resource\n- resource: https://auth.jampp.com\n  authorization_servers: [https://auth.jampp.com]\n  bearer_methods_supported: [header]\n  source: https://auth.jampp.com/.well-known/oauth-protected-resource\nobserved:\n- request: POST https://reporting-api.jampp.com/v1/graphql with no Authorization header\n  status: 401\n  body: '{\"error\":\"Neither Cookie nor Authorization\
  \ present.\"}'\n  fetched: '2026-08-12'\n- request: POST https://auth.jampp.com/v1/oauth/token with a JSON body\n  status: 400\n  body: '{\"error\":{\"message\":\"Invalid request: content must be application/x-www-form-urlencoded\"}}'\n  fetched: '2026-08-12'\n  note: The token endpoint rejects JSON; the form encoding is mandatory as documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jampp/refs/heads/main/authentication/jampp-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Advertising
- Marketing
- Mobile
- Analytics
- Reporting
- GraphQL
- Demand-Side Platform
- App Marketing
- Attribution
---
