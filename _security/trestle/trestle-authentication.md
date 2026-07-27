---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- http
description: Trestle has no OpenAPI, so this profile is assembled from the published documentation and the live OIDC discovery document rather than derived from securitySchemes. One IdentityServer fronts every Trestle surface; the scope selects which product surface the credential is good for (api = Web API and Participant Reporting; rets = RETS). Credentials are issued only after a per-MLS data licence contract is executed, so the auth model is fully documented but not self-service.
kind: authentication
layout: security
method: searched
name: Trestle Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Trestle secures its APIs with oauth2, openIdConnect, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Trestle
provider_slug: trestle
scheme_count: 4
schemes:
- applies_to:
  - Trestle RESO Web API (https://api.cotality.com/trestle/odata)
  - Trestle Participant Reporting API (WebAPI feeds)
  flow: clientCredentials
  name: TrestleWebAPIOAuth2
  parameters:
  - client_id
  - client_secret
  - grant_type=client_credentials
  - scope=api
  request_content_type: application/x-www-form-urlencoded
  sources:
  - https://trestle-documentation.corelogic.com/webapi.html
  token_lifetime_seconds: 28800
  token_type: Bearer
  token_url: https://api.cotality.com/trestle/oidc/connect/token
  type: oauth2
- applies_to:
  - Trestle RETS (https://api.cotality.com/trestle/rets)
  - Trestle Participant Reporting API (RETS feeds)
  flow: clientCredentials
  name: TrestleRETSOAuth2
  note: scope=api is rejected on RETS credentials (documented 400).
  parameters:
  - client_id
  - client_secret
  - grant_type=client_credentials
  - scope=rets
  sources:
  - https://trestle-documentation.corelogic.com/rets.html
  token_type: Bearer
  token_url: https://api.cotality.com/trestle/oidc/connect/token
  type: oauth2
- applies_to:
  - Trestle RETS
  detail: Base64-encoded client_id:client_secret in the Authorization header.
  name: TrestleRETSBasic
  note: Digest authentication is explicitly NOT supported. RETS is session-less — the login endpoint need not be called before Search/GetObject.
  scheme: basic
  sources:
  - https://trestle-documentation.corelogic.com/rets.html
  type: http
- applies_to:
  - Trestle Direct Web API (Matrix CRM + MLO)
  detail: OpenID Connect against the same Trestle IdentityServer, with Clareity Single Sign-On authorization and HTTP Basic named as alternatives. Access is further constrained by the acting user's privileges inside Matrix.
  name: TrestleDirectWebAPIOIDC
  sources:
  - https://trestle-documentation.corelogic.com/direct-webapi-crm-reference.html
  type: openIdConnect
slug: trestle-authentication
source_filename: trestle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  https://trestle-documentation.corelogic.com/webapi.html (Authentication),\n  https://trestle-documentation.corelogic.com/rets.html (Authentication),\n  https://trestle-documentation.corelogic.com/participant-reporting-api.html,\n  https://trestle-documentation.corelogic.com/direct-webapi-crm-reference.html,\n  plus the live OIDC discovery document at\n  https://api.cotality.com/trestle/oidc/.well-known/openid-configuration\n  (saved verbatim at well-known/trestle-openid-configuration.json).\ndocs: https://trestle-documentation.corelogic.com/webapi.html\ndescription: >-\n  Trestle has no OpenAPI, so this profile is assembled from the published\n  documentation and the live OIDC discovery document rather than derived from\n  securitySchemes. One IdentityServer fronts every Trestle surface; the scope\n  selects which product surface the credential is good for (api = Web API and\n  Participant Reporting; rets = RETS). Credentials\
  \ are issued only after a\n  per-MLS data licence contract is executed, so the auth model is fully\n  documented but not self-service.\n\nsummary:\n  types: [oauth2, openIdConnect, http]\n  oauth2_flows: [clientCredentials]\n  http_schemes: [basic, bearer]\n  api_key_in: []\n  self_service_credentials: false\n  credential_issuance: >-\n    Register a Technology Provider or Broker account at\n    https://trestle.corelogic.com, request a connection to each multiple listing\n    organization, and complete an e-signed data licence contract signed by all\n    parties. Credentials are scoped to a specific product/feed-type pair.\n\nissuer:\n  issuer: https://api.cotality.com\n  discovery: https://api.cotality.com/trestle/oidc/.well-known/openid-configuration\n  discovery_status: 200\n  jwks_uri: https://trestle-auth-prd.kfusw1prd.solutions.corelogic.com/.well-known/openid-configuration/jwks\n  jwks_file: well-known/trestle-openid-jwks.json\n  token_endpoint: https://trestle-auth-prd.kfusw1prd.solutions.corelogic.com/connect/token\n\
  \  documented_token_endpoint: https://api.cotality.com/trestle/oidc/connect/token\n  authorization_endpoint: https://trestle-auth-prd.kfusw1prd.solutions.corelogic.com/connect/authorize\n  introspection_endpoint: https://trestle-auth-prd.kfusw1prd.solutions.corelogic.com/connect/introspect\n  revocation_endpoint: https://trestle-auth-prd.kfusw1prd.solutions.corelogic.com/connect/revocation\n  userinfo_endpoint: https://trestle-auth-prd.kfusw1prd.solutions.corelogic.com/connect/userinfo\n  device_authorization_endpoint: https://trestle-auth-prd.kfusw1prd.solutions.corelogic.com/connect/deviceauthorization\n  end_session_endpoint: https://trestle-auth-prd.kfusw1prd.solutions.corelogic.com/connect/endsession\n  grant_types_supported: [authorization_code, client_credentials, refresh_token, implicit, 'urn:ietf:params:oauth:grant-type:device_code']\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  id_token_signing_alg_values_supported: [RS256]\n  code_challenge_methods_supported:\
  \ [plain, S256]\n  subject_types_supported: [public]\n  claims_supported: []\n  note: >-\n    The documented token URL (api.cotality.com/trestle/oidc/connect/token) and\n    the discovery-advertised endpoints point at different hostnames; the\n    solutions.corelogic.com auth host does not resolve publicly, so integrators\n    should use the documented api.cotality.com path.\n\nschemes:\n  - name: TrestleWebAPIOAuth2\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://api.cotality.com/trestle/oidc/connect/token\n    request_content_type: application/x-www-form-urlencoded\n    parameters: [client_id, client_secret, grant_type=client_credentials, scope=api]\n    token_type: Bearer\n    token_lifetime_seconds: 28800\n    applies_to:\n      - Trestle RESO Web API (https://api.cotality.com/trestle/odata)\n      - Trestle Participant Reporting API (WebAPI feeds)\n    sources: [https://trestle-documentation.corelogic.com/webapi.html]\n  - name: TrestleRETSOAuth2\n    type:\
  \ oauth2\n    flow: clientCredentials\n    token_url: https://api.cotality.com/trestle/oidc/connect/token\n    parameters: [client_id, client_secret, grant_type=client_credentials, scope=rets]\n    token_type: Bearer\n    applies_to:\n      - Trestle RETS (https://api.cotality.com/trestle/rets)\n      - Trestle Participant Reporting API (RETS feeds)\n    note: scope=api is rejected on RETS credentials (documented 400).\n    sources: [https://trestle-documentation.corelogic.com/rets.html]\n  - name: TrestleRETSBasic\n    type: http\n    scheme: basic\n    detail: Base64-encoded client_id:client_secret in the Authorization header.\n    applies_to: [Trestle RETS]\n    note: Digest authentication is explicitly NOT supported. RETS is session-less — the login endpoint need not be called before Search/GetObject.\n    sources: [https://trestle-documentation.corelogic.com/rets.html]\n  - name: TrestleDirectWebAPIOIDC\n    type: openIdConnect\n    detail: >-\n      OpenID Connect against the same\
  \ Trestle IdentityServer, with Clareity\n      Single Sign-On authorization and HTTP Basic named as alternatives. Access\n      is further constrained by the acting user's privileges inside Matrix.\n    applies_to: [Trestle Direct Web API (Matrix CRM + MLO)]\n    sources: [https://trestle-documentation.corelogic.com/direct-webapi-crm-reference.html]\n\ntoken_usage:\n  header: 'Authorization: Bearer <access_token>'\n  response_fields: [access_token, expires_in, token_type]\n  expires_in: 28800\n  guidance: >-\n    Documentation recommends caching the token and its expiry and refreshing\n    only when necessary; a token is valid for up to 8 hours.\n\nobserved:\n  - request: 'GET https://api.cotality.com/trestle/odata'\n    status: 200\n    note: OData service document answers anonymously.\n  - request: 'GET https://api.cotality.com/trestle/odata/$metadata'\n    status: 401\n    note: 'www-authenticate: Bearer — the CSDL contract itself is gated.'\n  - request: 'GET https://api.cotality.com/trestle/rets/login'\n\
  \    status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trestle/refs/heads/main/authentication/trestle-authentication.yml
summary_line: oauth2/openIdConnect/http · 4 schemes
tags:
- Real Estate
- United States
- MLS
- RESO
- Property Listings
- IDX
- PropTech
- Data Distribution
- OData
- RETS
- Listing Syndication
---
