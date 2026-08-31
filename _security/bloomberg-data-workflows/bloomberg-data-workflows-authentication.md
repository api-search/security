---
api_key_in: []
auth_types: []
description: Bloomberg's data-workflow surface carries three distinct and unrelated authentication models. There is no OpenAPI to derive securitySchemes from, so every statement here was observed on a live anonymous request or read from a first-party discovery document.
kind: authentication
layout: security
method: probed
name: Bloomberg Data Workflows Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bloomberg Data Workflows declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Bloomberg Data Workflows
provider_slug: bloomberg-data-workflows
scheme_count: 3
schemes:
- api: Bloomberg Data License API (REST / Hypermedia API)
  base_path: /eap/
  bearer_format: JWT
  host: https://api.bloomberg.com
  id: dl-rest-jwt
  location: request header (a query-string form is also accepted)
  note: 'The 401 names the mechanism exactly: every request must carry a JWT. Credentials are issued per-customer as a downloadable credential file from the DATA <GO> portal; the JWT is signed client-side per request (RFC 7519), it is not a long-lived bearer token fetched from a token endpoint. No anonymous token endpoint, no client-credentials flow, and no public sandbox credential exists.'
  observed:
    body: '{"error":"unauthorized_client","error_description":"No definition of jwt found in header or query string.","errors":[{"errorCode":"unauthorized-client","status":401}]}'
    status: 401
    url: https://api.bloomberg.com/eap/catalogs/
  scheme: bearer
  type: http
- api: Bloomberg.com web identity + entitlements
  authorization_endpoint: https://login.bloomberg.com/api/oauth/authorize
  grant_types:
  - authorization_code
  - refresh_token
  id: bloomberg-com-oidc
  id_token_signing_alg:
  - RS256
  issuer: https://www.bloomberg.com
  jwks_uri: https://login.bloomberg.com/api/oauth/.well-known/jwks.json
  note: This is the bloomberg.com consumer/subscriber identity provider — authorization code with mandatory PKCE, refresh tokens, and an `entitlements` scope. It is NOT the Data License or Server API authentication path; do not send these tokens to api.bloomberg.com. Recorded because it is the only OAuth surface Bloomberg publishes anonymously, and because it is a real, RFC 8414 + OIDC-discovery-conformant deployment.
  observed:
    status: 200
    url: https://www.bloomberg.com/.well-known/openid-configuration
  openid_connect_url: https://www.bloomberg.com/.well-known/openid-configuration
  pkce:
  - S256
  response_types:
  - code
  scopes:
  - openid
  - user
  - entitlements
  subject_types:
  - public
  token_endpoint: https://login.bloomberg.com/api/oauth/token
  type: openIdConnect
- api: Bloomberg Server API (SAPI) / Desktop API / B-PIPE
  docs: https://bloomberg.github.io/blpapi-docs/
  id: blpapi-session
  location: transport
  note: BLPAPI is not HTTP. Clients open a TCP session with the BLPAPI SDK — localhost:8194 for the Desktop API, or the customer's own SAPI/B-PIPE host and port. Identity is the Terminal entitlement of the logged-in user (Desktop API) or, for SAPI/B-PIPE, an application name plus the customer-provisioned TLS/PKCS#12 credentials issued by Bloomberg. There is no API key, no bearer token and no public credential of any kind; access requires an active Bloomberg Professional or Enterprise agreement.
  type: mutualTLS
slug: bloomberg-data-workflows-authentication
source_filename: bloomberg-data-workflows-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: >-\n  Live probes of https://api.bloomberg.com/eap/catalogs/ and\n  https://www.bloomberg.com/.well-known/openid-configuration, plus\n  https://professional.bloomberg.com/support/api-library/\ndescription: >-\n  Bloomberg's data-workflow surface carries three distinct and unrelated authentication models.\n  There is no OpenAPI to derive securitySchemes from, so every statement here was observed on a\n  live anonymous request or read from a first-party discovery document.\nschemes:\n  - id: dl-rest-jwt\n    api: Bloomberg Data License API (REST / Hypermedia API)\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    location: request header (a query-string form is also accepted)\n    host: https://api.bloomberg.com\n    base_path: /eap/\n    observed:\n      url: https://api.bloomberg.com/eap/catalogs/\n      status: 401\n      body: >-\n        {\"error\":\"unauthorized_client\",\"error_description\":\"No definition\
  \ of jwt found in header\n        or query string.\",\"errors\":[{\"errorCode\":\"unauthorized-client\",\"status\":401}]}\n    note: >-\n      The 401 names the mechanism exactly: every request must carry a JWT. Credentials are issued\n      per-customer as a downloadable credential file from the DATA <GO> portal; the JWT is signed\n      client-side per request (RFC 7519), it is not a long-lived bearer token fetched from a token\n      endpoint. No anonymous token endpoint, no client-credentials flow, and no public sandbox\n      credential exists.\n  - id: bloomberg-com-oidc\n    api: Bloomberg.com web identity + entitlements\n    type: openIdConnect\n    openid_connect_url: https://www.bloomberg.com/.well-known/openid-configuration\n    issuer: https://www.bloomberg.com\n    authorization_endpoint: https://login.bloomberg.com/api/oauth/authorize\n    token_endpoint: https://login.bloomberg.com/api/oauth/token\n    jwks_uri: https://login.bloomberg.com/api/oauth/.well-known/jwks.json\n\
  \    grant_types: [authorization_code, refresh_token]\n    response_types: [code]\n    pkce: [S256]\n    id_token_signing_alg: [RS256]\n    subject_types: [public]\n    scopes: [openid, user, entitlements]\n    observed:\n      url: https://www.bloomberg.com/.well-known/openid-configuration\n      status: 200\n    note: >-\n      This is the bloomberg.com consumer/subscriber identity provider — authorization code with\n      mandatory PKCE, refresh tokens, and an `entitlements` scope. It is NOT the Data License or\n      Server API authentication path; do not send these tokens to api.bloomberg.com. Recorded\n      because it is the only OAuth surface Bloomberg publishes anonymously, and because it is a\n      real, RFC 8414 + OIDC-discovery-conformant deployment.\n  - id: blpapi-session\n    api: Bloomberg Server API (SAPI) / Desktop API / B-PIPE\n    type: mutualTLS\n    location: transport\n    note: >-\n      BLPAPI is not HTTP. Clients open a TCP session with the BLPAPI SDK — localhost:8194\
  \ for the\n      Desktop API, or the customer's own SAPI/B-PIPE host and port. Identity is the Terminal\n      entitlement of the logged-in user (Desktop API) or, for SAPI/B-PIPE, an application name\n      plus the customer-provisioned TLS/PKCS#12 credentials issued by Bloomberg. There is no API\n      key, no bearer token and no public credential of any kind; access requires an active\n      Bloomberg Professional or Enterprise agreement.\n    docs: https://bloomberg.github.io/blpapi-docs/\npublic_credential_available: false\napi_keys: false\noauth2_client_credentials: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-data-workflows/refs/heads/main/authentication/bloomberg-data-workflows-authentication.yml
summary_line: 3 schemes
tags:
- Enterprise Data
- Financial Analytics
- Financial-Services
- Investment Management
- Market Data
- Reference Data
- Trading
---
