---
api_key_in: []
api_specs:
- filename: public
  format: yaml
  label: Yahoo DSP Traffic API
  slug: dsp-traffic-api
  spec_type: Postman
  url: https://www.postman.com/yahoodsp/workspace/public
auth_types: []
description: Yahoo authenticates every public API surface with OAuth 2.0, but the flows differ sharply by product. Consumer-facing APIs (Fantasy Sports, Sign In With Yahoo) use the three-legged authorization-code flow against the Yahoo identity service at api.login.yahoo.com, which also publishes a full OpenID Connect Discovery document. The ad-tech APIs (DSP Traffic, DSP Reporting, DataX, Conversion API) use a two-legged client_credentials flow in which the client authenticates with a self-signed JWT and the resulting bearer token is presented in Yahoo's own X-Auth-Token / X-Auth-Method header pair rather than in Authorization.
kind: authentication
layout: security
method: searched
name: Yahoo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yahoo declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Yahoo
provider_slug: yahoo
scheme_count: 3
schemes:
- applies_to:
  - Yahoo Fantasy Sports API
  - Sign In With Yahoo
  authorization_endpoint: https://api.login.yahoo.com/oauth2/request_auth
  docs: https://developer.yahoo.com/oauth2/guide/flows_authcode/
  evidence: https://api.login.yahoo.com/.well-known/openid-configuration (HTTP 200)
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  id: yahoo-oauth2-authorization-code
  id_token_signing_algs:
  - ES256
  - RS256
  introspection_endpoint: https://api.login.yahoo.com/oauth2/introspect
  jwks_uri: https://api.login.yahoo.com/openid/v1/certs
  registration: https://developer.yahoo.com/apps/create/
  revocation_endpoint: https://api.login.yahoo.com/oauth2/revoke
  token_endpoint: https://api.login.yahoo.com/oauth2/get_token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  token_placement: 'Authorization: Bearer <access_token>'
  type: oauth2
  userinfo_endpoint: https://api.login.yahoo.com/openid/v1/userinfo
- acr_values:
  - AAL1
  - AAL2
  applies_to:
  - Sign In With Yahoo
  claims:
  - aud
  - email
  - email_verified
  - birthdate
  - exp
  - family_name
  - given_name
  - iat
  - iss
  - locale
  - name
  - sub
  - auth_time
  claims_parameter_supported: false
  discovery: https://api.login.yahoo.com/.well-known/openid-configuration
  docs: https://developer.yahoo.com/oauth2/guide/openid_connect/
  evidence: https://api.login.yahoo.com/.well-known/openid-configuration (HTTP 200)
  id: yahoo-openid-connect
  issuer: https://api.login.yahoo.com
  request_parameter_supported: false
  request_uri_parameter_supported: false
  response_modes:
  - query
  response_types:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  subject_types:
  - public
  type: openIdConnect
- applies_to:
  - Yahoo DSP Traffic API
  - Yahoo DSP Reporting API
  - Yahoo Conversion API
  - Yahoo Ad Tech DataX API
  client_assertion: A JSON Web Token signed by the client identifies it to the token endpoint. DSP signs with HS256 using the client secret; DataX exchanges an RSA public key generated with OpenSSL and emailed to dataoperations@yahooinc.com during onboarding.
  credential_issuance: Client ID and client secret are issued once, in the DSP UI (My Account > Activate), and are never redisplayed. A seat user must be created and API-enabled by a User Ops role holder before credentials can be generated.
  docs: https://help.yahooinc.com/dsp-api/docs/setup-access-guide
  evidence: https://help.yahooinc.com/dsp-api/docs/authorization-and-headers (HTTP 200)
  flow: clientCredentials
  id: yahoo-dsp-client-credentials-jwt
  token_endpoint: https://id.b2b.yahooincapis.com/zts/v1/oauth2/token
  token_placement: 'X-Auth-Method: OAuth2 and X-Auth-Token: <access token> headers, alongside Content-Type: application/json. The DSP APIs do NOT read the Authorization header.'
  token_ttl_note: DataX raised the access-token TTL from 3600s to 21600s; clients are REQUIRED to cache and reuse tokens and read expires_in rather than assume the default.
  token_ttl_seconds: 21600
  type: oauth2
slug: yahoo-authentication
source_filename: yahoo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Yahoo\nproviderId: yahoo\ngenerated: '2026-08-28'\nmethod: searched\nsource: >-\n  https://developer.yahoo.com/oauth2/guide/ ,\n  https://api.login.yahoo.com/.well-known/openid-configuration ,\n  https://help.yahooinc.com/dsp-api/docs/authentication ,\n  https://help.yahooinc.com/dsp-api/docs/setup-access-guide ,\n  https://help.yahooinc.com/dsp-api/docs/authorization-and-headers ,\n  https://help.yahooinc.com/datax/docs/security-authentication\ndocs:\n  - https://developer.yahoo.com/oauth2/guide/\n  - https://help.yahooinc.com/dsp-api/docs/setup-access-guide\n  - https://help.yahooinc.com/datax/docs/security-authentication\ndescription: >-\n  Yahoo authenticates every public API surface with OAuth 2.0, but the flows differ sharply by\n  product. Consumer-facing APIs (Fantasy Sports, Sign In With Yahoo) use the three-legged\n  authorization-code flow against the Yahoo identity service at api.login.yahoo.com,\
  \ which also\n  publishes a full OpenID Connect Discovery document. The ad-tech APIs (DSP Traffic, DSP\n  Reporting, DataX, Conversion API) use a two-legged client_credentials flow in which the client\n  authenticates with a self-signed JWT and the resulting bearer token is presented in Yahoo's own\n  X-Auth-Token / X-Auth-Method header pair rather than in Authorization.\nschemes:\n  - id: yahoo-oauth2-authorization-code\n    type: oauth2\n    flow: authorizationCode\n    applies_to:\n      - Yahoo Fantasy Sports API\n      - Sign In With Yahoo\n    authorization_endpoint: https://api.login.yahoo.com/oauth2/request_auth\n    token_endpoint: https://api.login.yahoo.com/oauth2/get_token\n    introspection_endpoint: https://api.login.yahoo.com/oauth2/introspect\n    revocation_endpoint: https://api.login.yahoo.com/oauth2/revoke\n    userinfo_endpoint: https://api.login.yahoo.com/openid/v1/userinfo\n    jwks_uri: https://api.login.yahoo.com/openid/v1/certs\n    grant_types:\n      - authorization_code\n\
  \      - refresh_token\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n    id_token_signing_algs:\n      - ES256\n      - RS256\n    token_placement: 'Authorization: Bearer <access_token>'\n    registration: https://developer.yahoo.com/apps/create/\n    docs: https://developer.yahoo.com/oauth2/guide/flows_authcode/\n    evidence: https://api.login.yahoo.com/.well-known/openid-configuration (HTTP 200)\n  - id: yahoo-openid-connect\n    type: openIdConnect\n    applies_to:\n      - Sign In With Yahoo\n    issuer: https://api.login.yahoo.com\n    discovery: https://api.login.yahoo.com/.well-known/openid-configuration\n    subject_types:\n      - public\n    response_types:\n      - code\n      - token\n      - id_token\n      - code token\n      - code id_token\n      - token id_token\n      - code token id_token\n    response_modes:\n      - query\n    acr_values:\n      - AAL1\n      - AAL2\n    claims:\n      - aud\n      - email\n      - email_verified\n\
  \      - birthdate\n      - exp\n      - family_name\n      - given_name\n      - iat\n      - iss\n      - locale\n      - name\n      - sub\n      - auth_time\n    claims_parameter_supported: false\n    request_parameter_supported: false\n    request_uri_parameter_supported: false\n    docs: https://developer.yahoo.com/oauth2/guide/openid_connect/\n    evidence: https://api.login.yahoo.com/.well-known/openid-configuration (HTTP 200)\n  - id: yahoo-dsp-client-credentials-jwt\n    type: oauth2\n    flow: clientCredentials\n    applies_to:\n      - Yahoo DSP Traffic API\n      - Yahoo DSP Reporting API\n      - Yahoo Conversion API\n      - Yahoo Ad Tech DataX API\n    token_endpoint: https://id.b2b.yahooincapis.com/zts/v1/oauth2/token\n    client_assertion: >-\n      A JSON Web Token signed by the client identifies it to the token endpoint. DSP signs with\n      HS256 using the client secret; DataX exchanges an RSA public key generated with OpenSSL and\n      emailed to dataoperations@yahooinc.com\
  \ during onboarding.\n    token_placement: >-\n      X-Auth-Method: OAuth2 and X-Auth-Token: <access token> headers, alongside\n      Content-Type: application/json. The DSP APIs do NOT read the Authorization header.\n    token_ttl_seconds: 21600\n    token_ttl_note: >-\n      DataX raised the access-token TTL from 3600s to 21600s; clients are REQUIRED to cache and\n      reuse tokens and read expires_in rather than assume the default.\n    credential_issuance: >-\n      Client ID and client secret are issued once, in the DSP UI (My Account > Activate), and are\n      never redisplayed. A seat user must be created and API-enabled by a User Ops role holder\n      before credentials can be generated.\n    docs: https://help.yahooinc.com/dsp-api/docs/setup-access-guide\n    evidence: https://help.yahooinc.com/dsp-api/docs/authorization-and-headers (HTTP 200)\nnotes:\n  - >-\n    The Yahoo Conversion API requires its own separate direct OAuth 2.0 setup even for callers\n    already authenticated\
  \ against the DSP Traffic API.\n  - >-\n    Yahoo publishes no OpenAPI/Swagger description for any of these surfaces, so this profile is\n    searched from the published documentation rather than derived from securitySchemes.\n  - >-\n    The DSP token endpoint id.b2b.yahooincapis.com/zts/v1 is an Athenz ZTS deployment; Athenz is\n    Yahoo's own open-source service-authentication project (github.com/AthenZ).\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yahoo/refs/heads/main/authentication/yahoo-authentication.yml
summary_line: 3 schemes
tags:
- Advertising
- Programmatic Advertising
- Demand Side Platform
- Fantasy Sports
- Sports Data
- Identity
- OpenID Connect
- OAuth
- Audience Data
- Media
- Reporting
- Conversion Tracking
---
