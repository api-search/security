---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Zemanta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zemanta declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Zemanta
provider_slug: zemanta
scheme_count: 2
schemes:
- applied_to: all /rest/v1/ operations
  evidence: '"Teads DSP REST API uses two-legged OAuth2 authentication using client credentials." POST https://oneapi.zemanta.com/o/token/ with Authorization: Basic base64(client_id:client_secret) and body grant_type=client_credentials returns {"access_token": ..., "token_type": "Bearer", "expires_in": 36000, "scope": "read write"}.'
  flow: clientCredentials
  grant_type: client_credentials
  key: oauth2ClientCredentials
  scopes:
  - read
  - write
  token_endpoint_auth_method: client_secret_basic
  token_lifetime_note: Access tokens are valid for 10 hours; the docs instruct clients to cache and reuse the token for the duration of its validity rather than re-issuing per call.
  token_lifetime_seconds: 36000
  token_request_content_type: application/x-www-form-urlencoded
  token_type: Bearer
  token_url: https://oneapi.zemanta.com/o/token/
  type: oauth2
- applied_to: all /rest/v1/ operations
  evidence: '"The client credentials are used to acquire an access token, which must then be passed to all REST API calls as the header Authorization: Bearer <access_token>"'
  format: Bearer <access_token>
  header: Authorization
  key: bearerToken
  scheme: bearer
  type: http
slug: zemanta-authentication
source_filename: zemanta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://dev.zemanta.com/one/api/\ndocs: https://dev.zemanta.com/one/api/\napi: zemanta:teads-dsp-api\nsummary: >-\n  The Teads DSP REST API (formerly the Zemanta One API) uses two-legged OAuth 2.0\n  with the client_credentials grant. Client credentials are self-issued from the\n  DSP console; the resulting bearer token is presented on every REST call.\nschemes:\n- key: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://oneapi.zemanta.com/o/token/\n  token_endpoint_auth_method: client_secret_basic\n  token_request_content_type: application/x-www-form-urlencoded\n  grant_type: client_credentials\n  scopes:\n  - read\n  - write\n  token_type: Bearer\n  token_lifetime_seconds: 36000\n  token_lifetime_note: >-\n    Access tokens are valid for 10 hours; the docs instruct clients to cache and\n    reuse the token for the duration of its validity rather than re-issuing per call.\n  applied_to:\
  \ all /rest/v1/ operations\n  evidence: >-\n    \"Teads DSP REST API uses two-legged OAuth2 authentication using client credentials.\"\n    POST https://oneapi.zemanta.com/o/token/ with Authorization: Basic base64(client_id:client_secret)\n    and body grant_type=client_credentials returns {\"access_token\": ..., \"token_type\": \"Bearer\",\n    \"expires_in\": 36000, \"scope\": \"read write\"}.\n- key: bearerToken\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Bearer <access_token>'\n  applied_to: all /rest/v1/ operations\n  evidence: >-\n    \"The client credentials are used to acquire an access token, which must then be\n    passed to all REST API calls as the header Authorization: Bearer <access_token>\"\ncredential_issuance:\n  self_service: partial\n  console_url: https://dsp.outbrain.com/o/applications/\n  steps:\n  - Log in to the Teads DSP console (one.zemanta.com now 301-redirects to dsp.outbrain.com).\n  - Open https://dsp.outbrain.com/o/applications/ and\
  \ click \"New Application\".\n  - Name the application and save; the resulting Client ID and Client Secret are the API credentials.\n  gate: >-\n    API access itself is sales-gated — \"In order to use Teads DSP REST API, please contact\n    your sales representative.\" The credential-creation screen is only reachable by an\n    authenticated DSP customer.\n  support_contact: api-support@zemanta.com\nprobes:\n- url: https://oneapi.zemanta.com/o/token/\n  method: POST\n  http_status: 405\n  note: GET/HEAD rejected; the route exists.\n- url: https://dsp.outbrain.com/o/token/\n  method: POST\n  body: grant_type=client_credentials\n  http_status: 401\n  response: '{\"error\": \"invalid_client\"}'\n  headers_observed:\n  - 'www-authenticate: Bearer error=\"invalid_client\"'\n  note: >-\n    Live, anonymous confirmation that the OAuth2 token endpoint is deployed and speaks\n    RFC 6749 / RFC 6750 error semantics. dsp.outbrain.com is the same Django application\n    as oneapi.zemanta.com (both\
  \ emit the x_z1_trace_id header, \"z1\" = Zemanta One).\nnotes:\n- No API-key, mutualTLS or OpenID Connect scheme is documented for this API.\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server document is served on any Zemanta host (see well-known/zemanta-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zemanta/refs/heads/main/authentication/zemanta-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Advertising
- Native Advertising
- Programmatic
- DSP
- AdTech
- Content Recommendation
- Marketing
- Campaign Management
- Demand Side Platform
- Media Buying
---
