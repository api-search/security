---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
- mutualTLS
- http
- x509-certificate
- jwt-second-factor
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Discover Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Discover secures its APIs with oauth2, mutualTLS, http, x509-certificate, and jwt-second-factor across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Discover
provider_slug: discover
scheme_count: 4
schemes:
- client_authentication: HTTP Basic (base64 client_id:client_secret) or form body
  expires_in_seconds: 3600
  flow: clientCredentials
  name: OAuth2ClientCredentials
  request_content_type: application/x-www-form-urlencoded
  required_body: grant_type=client_credentials&scope=<SCOPE_NAME>
  required_headers:
  - X-DFS-API-PLAN
  source_section: 5. How to use OAuth 2 - Client Credentials
  token_type: Bearer
  token_url: https://apis.discover.com/auth/oauth/v2/token
  type: oauth2
  usage: 'Authorization: Bearer <access_token>'
- description: A JWS token the partner signs with its registered PARTNER_SIGNATURE_CERT private key and sends as a second authentication factor on APIs that require it. Header carries typ, alg (RS256) and kid; claims include a SHA-256 content_hash of the request body.
  header: X-DFS-C-APP-JWT
  in: header
  name: SecondFactorJWT
  source_section: 7. How to use Second Factor JWT
  type: jwt
- description: A Discover-issued consumer application certificate presented as a second authentication factor on APIs that require it.
  header: X-DFS-C-APP-CERT
  in: header
  name: ConsumerApplicationCertificate
  source_section: 6. How to use Consumer Application Certificate
  type: x509-certificate
- description: mTLS with a partner-supplied X.509 SSL certificate, used per API and for Discover's outgoing (webhook / notification) calls back to the partner.
  name: MutualTLS
  source_section: 3. Security Methods Overview / 9. Outgoing API Authentication
  type: mutualTLS
slug: discover-authentication
source_filename: discover-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://partner.discoverglobalnetwork.com/going-live-with-discover?tab=developer-guide\ndocs: https://partner.discoverglobalnetwork.com/going-live-with-discover?tab=developer-guide\nnote: >-\n  Discover publishes no OpenAPI, so nothing here is derived from a spec. Every field below is read\n  from the Discover Partner Product Portal developer guide, which is public and server-rendered,\n  and from live anonymous probes of apis.discover.com. Section numbers refer to that guide.\nsummary:\n  types: [oauth2, mutualTLS, http, x509-certificate, jwt-second-factor]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  payload_security: [JWE, JWS, nested-JWT-JWS-in-JWE, field-level-encryption]\n  transport: TLS 1.2 or TLS 1.3 required\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://apis.discover.com/auth/oauth/v2/token\n  token_type: Bearer\n  expires_in_seconds: 3600\n\
  \  client_authentication: HTTP Basic (base64 client_id:client_secret) or form body\n  request_content_type: application/x-www-form-urlencoded\n  required_body: grant_type=client_credentials&scope=<SCOPE_NAME>\n  required_headers:\n  - X-DFS-API-PLAN\n  usage: 'Authorization: Bearer <access_token>'\n  source_section: '5. How to use OAuth 2 - Client Credentials'\n- name: SecondFactorJWT\n  type: jwt\n  in: header\n  header: X-DFS-C-APP-JWT\n  description: >-\n    A JWS token the partner signs with its registered PARTNER_SIGNATURE_CERT private key and sends\n    as a second authentication factor on APIs that require it. Header carries typ, alg (RS256) and\n    kid; claims include a SHA-256 content_hash of the request body.\n  source_section: '7. How to use Second Factor JWT'\n- name: ConsumerApplicationCertificate\n  type: x509-certificate\n  in: header\n  header: X-DFS-C-APP-CERT\n  description: A Discover-issued consumer application certificate presented as a second\n    authentication\
  \ factor on APIs that require it.\n  source_section: '6. How to use Consumer Application Certificate'\n- name: MutualTLS\n  type: mutualTLS\n  description: >-\n    mTLS with a partner-supplied X.509 SSL certificate, used per API and for Discover's outgoing\n    (webhook / notification) calls back to the partner.\n  source_section: '3. Security Methods Overview / 9. Outgoing API Authentication'\npayload_protection:\n  jwe:\n    purpose: payload and field-level encryption of requests and responses\n    keys: Discover JWE public key + partner JWE public key exchanged at registration\n  jws:\n    purpose: payload signature and non-repudiation; Discover also signs its responses\n    algorithm: RS256\n  nested_jwt: JWS signed payload nested inside a JWE (JWS-in-JWE)\n  hashing: SHA-256 content_hash claim over the UTF-8 request body\njwks:\n  endpoints:\n  - url: https://apis.discover.com/dfs/jwk/v1/public-keys\n    status: 200\n    anonymous: true\n    probed: '2026-09-06'\n  - url: https://apis.discover.com/dfs/certs/v1/jwks.json?client_id=<your_client_id>\n\
  \    status: 200\n    anonymous: true\n    probed: '2026-09-06'\n    note: the documented form takes a client_id query parameter; the bare path also answers 200\n  - url: https://sandbox.apis.discover.com/dfs/jwk/v1/public-keys\n    status: 200\n    anonymous: true\n    probed: '2026-09-06'\n  file: authentication/discover-jwks.json\n  key_rotation: JWKS endpoint keys expire every 90 days\n  key_uses: [sig, enc]\nper_api_security:\n  note: read from the \"Security Methods Overview\" table in section 3 of the developer guide\n  matrix:\n  - api: Discover Stored Token Services (DSTS)\n    request_authentication: OAuth 2 Client Credentials + Second Factor JWT\n    payload_encryption: JWE\n    outgoing_api_security: mTLS\n  - api: Side-by-Side Token Services (SXS)\n    request_authentication: OAuth 2 Client Credentials + Second Factor JWT\n    payload_encryption: JWE\n    outgoing_api_security: mTLS\n  - api: Discover Enhanced Decisioning (DED)\n    request_authentication: OAuth 2 Client Credentials\
  \ + Consumer Application Certificate\n    payload_encryption: null\n    outgoing_api_security: null\nidentity_provider:\n  partner_portal:\n    issuer: https://identity.discoverglobalnetwork.com/oauth2/default\n    org_issuer: https://identity.discoverglobalnetwork.com\n    vendor: Okta\n    discovery: well-known/discover-identity-openid-configuration.json\n    note: >-\n      This is the human sign-in for the Discover Partner Product Portal and Developer Center, not\n      the API gateway's token endpoint. API access tokens come from\n      https://apis.discover.com/auth/oauth/v2/token.\nonboarding:\n  self_service: false\n  detail: >-\n    \"Currently, portal access is by invitation only.\" Partners self-register at\n    developer.discover.com only after a Discover representative sends an invitation; client_id,\n    client_secret, API scopes, API plan and certificates are then issued per environment.\n  source: https://partner.discoverglobalnetwork.com/going-live-with-discover?tab=developer-guide\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/discover/refs/heads/main/authentication/discover-authentication.yml
summary_line: oauth2/mutualTLS/http/x509-certificate/jwt-second-factor · 4 schemes
tags:
- Credit Cards
- Payments
- Card Network
- Tokenization
- Financial Services
- Fraud
- Fortune 500
---
