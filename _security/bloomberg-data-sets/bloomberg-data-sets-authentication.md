---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- http
description: Bloomberg has no published OpenAPI, so this profile was NOT derived from a spec - it was read from the two machine-readable authorization-server metadata documents Bloomberg serves at www.bloomberg.com and login.bloomberg.com, and from the authentication challenge the Data License API itself returns to an anonymous client.
kind: authentication
layout: security
method: probed
name: Bloomberg Data Sets Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Bloomberg Data Sets secures its APIs with oauth2, openIdConnect, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Bloomberg Data Sets
provider_slug: bloomberg-data-sets
scheme_count: 3
schemes:
- authorization_endpoint: https://login.bloomberg.com/api/oauth/authorize
  code_challenge_methods_supported:
  - S256
  grant_types_supported:
  - authorization_code
  - refresh_token
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://www.bloomberg.com
  jwks_uri: https://login.bloomberg.com/api/oauth/.well-known/jwks.json
  name: BloombergOIDC
  openIdConnectUrl: https://www.bloomberg.com/.well-known/openid-configuration
  response_types_supported:
  - code
  scopes_supported:
  - openid
  - user
  - entitlements
  sources:
  - well-known/bloomberg-data-sets-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://login.bloomberg.com/api/oauth/token
  type: openIdConnect
- flows:
  - authorizationUrl: https://login.bloomberg.com/api/oauth/authorize
    flow: authorizationCode
    pkce: S256
    scopes:
    - openid
    - user
    - entitlements
    tokenUrl: https://login.bloomberg.com/api/oauth/token
  name: BloombergOAuth2
  rfc: RFC 8414 authorization server metadata
  sources:
  - well-known/bloomberg-data-sets-oauth-authorization-server.json
  type: oauth2
- applies_to: https://api.bloomberg.com/eap
  bearerFormat: JWT
  evidence: 'GET https://api.bloomberg.com/eap/catalogs/ returns HTTP 401 with {"error":"unauthorized_client","error_description":"No definition of jwt found in header or query string."} and the response advertises Access-Control-Allow-Origin: https://console.bloomberg.com. The JWT is issued against Data License credentials provisioned through the Bloomberg Enterprise Console, not through the public OIDC flow above.'
  name: DataLicenseJWT
  note: The token acquisition procedure for Data License / HAPI is documented only behind the Enterprise Console; it was NOT read, and nothing about its shape is asserted here beyond the header requirement the API itself states.
  scheme: bearer
  type: http
slug: bloomberg-data-sets-authentication
source_filename: bloomberg-data-sets-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: >-\n  https://www.bloomberg.com/.well-known/openid-configuration,\n  https://www.bloomberg.com/.well-known/oauth-authorization-server,\n  https://login.bloomberg.com/api/oauth/.well-known/jwks.json, and the live 401/403\n  envelopes returned by https://api.bloomberg.com/eap/ and /eap/catalogs/.\ndocs: https://professional.bloomberg.com/support/api-library/\ndescription: >-\n  Bloomberg has no published OpenAPI, so this profile was NOT derived from a spec - it\n  was read from the two machine-readable authorization-server metadata documents\n  Bloomberg serves at www.bloomberg.com and login.bloomberg.com, and from the\n  authentication challenge the Data License API itself returns to an anonymous client.\nsummary:\n  types:\n    - oauth2\n    - openIdConnect\n    - http\n  api_key_in: []\n  oauth2_flows:\n    - authorizationCode\n  http_schemes:\n    - bearer\n  pkce_required_methods:\n    - S256\nschemes:\n  - name: BloombergOIDC\n\
  \    type: openIdConnect\n    openIdConnectUrl: https://www.bloomberg.com/.well-known/openid-configuration\n    issuer: https://www.bloomberg.com\n    authorization_endpoint: https://login.bloomberg.com/api/oauth/authorize\n    token_endpoint: https://login.bloomberg.com/api/oauth/token\n    jwks_uri: https://login.bloomberg.com/api/oauth/.well-known/jwks.json\n    response_types_supported:\n      - code\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n    subject_types_supported:\n      - public\n    id_token_signing_alg_values_supported:\n      - RS256\n    code_challenge_methods_supported:\n      - S256\n    scopes_supported:\n      - openid\n      - user\n      - entitlements\n    sources:\n      - well-known/bloomberg-data-sets-openid-configuration.json\n  - name: BloombergOAuth2\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.bloomberg.com/api/oauth/authorize\n        tokenUrl: https://login.bloomberg.com/api/oauth/token\n\
  \        pkce: S256\n        scopes:\n          - openid\n          - user\n          - entitlements\n    rfc: RFC 8414 authorization server metadata\n    sources:\n      - well-known/bloomberg-data-sets-oauth-authorization-server.json\n  - name: DataLicenseJWT\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    applies_to: https://api.bloomberg.com/eap\n    evidence: >-\n      GET https://api.bloomberg.com/eap/catalogs/ returns HTTP 401 with\n      {\"error\":\"unauthorized_client\",\"error_description\":\"No definition of jwt found in\n      header or query string.\"} and the response advertises\n      Access-Control-Allow-Origin: https://console.bloomberg.com. The JWT is issued\n      against Data License credentials provisioned through the Bloomberg Enterprise\n      Console, not through the public OIDC flow above.\n    note: >-\n      The token acquisition procedure for Data License / HAPI is documented only behind\n      the Enterprise Console; it was NOT read, and nothing\
  \ about its shape is asserted\n      here beyond the header requirement the API itself states.\nobserved_challenges:\n  - url: https://api.bloomberg.com/eap/\n    status: 401\n    error: unauthorized_client\n    detail: No definition of jwt found in header or query string.\n  - url: https://api.bloomberg.com/eap/catalogs/\n    status: 401\n    error: unauthorized_client\n    detail: No definition of jwt found in header or query string.\n  - url: https://api.bloomberg.com/\n    status: 403\n    error: access_denied\n    detail: Access forbidden.\nnon_http_authentication:\n  - name: BLPAPI session authorization\n    note: >-\n      The Bloomberg Open API (BLPAPI) is not an HTTP API. Desktop API authorizes against\n      a logged-in Bloomberg Terminal on the local machine; Server API and B-PIPE\n      authorize sessions with an application name / identity token exchanged over the\n      BLPAPI wire protocol. There is no bearer header and no OAuth surface on that path.\n      Recorded for\
  \ completeness; no HTTP security scheme is claimed for it.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-data-sets/refs/heads/main/authentication/bloomberg-data-sets-authentication.yml
summary_line: oauth2/openIdConnect/http · 3 schemes
tags:
- Analytics
- Datasets
- Financial-Services
- Market Data
- Reference Data
- Historical Data
- Financial Data
- Data Licensing
---
