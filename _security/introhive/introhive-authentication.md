---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Introhive Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Introhive secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Introhive
provider_slug: introhive
scheme_count: 1
schemes:
- flows:
  - flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    response_types:
    - code
    scopes: {}
  instances:
  - authorizationUrl: https://app.introhive.com/oauth/authorize
    issuer: https://app.introhive.com
    region: us
    tokenUrl: https://app.introhive.com/oauth/token
  - authorizationUrl: https://ca.introhive.com/oauth/authorize
    issuer: https://ca.introhive.com
    region: ca
    tokenUrl: https://ca.introhive.com/oauth/token
  - authorizationUrl: https://uk.introhive.com/oauth/authorize
    issuer: https://uk.introhive.com
    region: uk
    tokenUrl: https://uk.introhive.com/oauth/token
  name: OAuth2
  sources:
  - well-known/introhive-oauth-authorization-server.json
  - well-known/introhive-ca-oauth-authorization-server.json
  - well-known/introhive-uk-oauth-authorization-server.json
  type: oauth2
slug: introhive-authentication
source_filename: introhive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: https://app.introhive.com/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  Derived verbatim from Introhive's own RFC 8414 OAuth 2.0 Authorization Server Metadata\n  documents, probed live on each regional platform host. There is no OpenAPI description\n  and no public authentication documentation page, so the profile below is exactly what\n  the discovery documents assert and nothing more. Scope semantics are not advertised\n  (no `scopes_supported` member), so no scopes/ artifact was written.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  pkce: true\n  pkce_methods:\n  - S256\n  refresh_tokens: true\n  client_authentication:\n  - client_secret_post\n  - client_secret_basic\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: OAuth2\n  type: oauth2\n  sources:\n  - well-known/introhive-oauth-authorization-server.json\n  - well-known/introhive-ca-oauth-authorization-server.json\n\
  \  - well-known/introhive-uk-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    response_types:\n    - code\n    grant_types:\n    - authorization_code\n    - refresh_token\n    scopes: {}\n  instances:\n  - region: us\n    issuer: https://app.introhive.com\n    authorizationUrl: https://app.introhive.com/oauth/authorize\n    tokenUrl: https://app.introhive.com/oauth/token\n  - region: ca\n    issuer: https://ca.introhive.com\n    authorizationUrl: https://ca.introhive.com/oauth/authorize\n    tokenUrl: https://ca.introhive.com/oauth/token\n  - region: uk\n    issuer: https://uk.introhive.com\n    authorizationUrl: https://uk.introhive.com/oauth/authorize\n    tokenUrl: https://uk.introhive.com/oauth/token\nclient_registration:\n  dynamic: false\n  console: https://app.introhive.com/oauth/applications\n  console_status: 302 to /application_session/sign_in — authenticated tenant admins only\n  note: >-\n    No RFC 7591 dynamic client registration endpoint is advertised.\
  \ OAuth applications are\n    registered inside the product by a signed-in administrator.\nobservations:\n- The three regional issuers are byte-for-byte identical apart from the host, indicating one\n  codebase deployed per data-residency region (US, Canada, UK).\n- Endpoint layout (/oauth/authorize, /oauth/token, /oauth/applications) matches the Doorkeeper\n  Rails OAuth provider, which is consistent with Introhive's published Ruby repositories.\n- 'PKCE is advertised with S256 only: no `plain` challenge method is offered.'\n- No token introspection (RFC 7662), revocation (RFC 7009), device authorization (RFC 8628),\n  or JWKS endpoint is advertised in the metadata.\nx-evidence:\n  fetched: '2026-08-01'\n  urls:\n  - https://app.introhive.com/.well-known/oauth-authorization-server\n  - https://ca.introhive.com/.well-known/oauth-authorization-server\n  - https://uk.introhive.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/introhive/refs/heads/main/authentication/introhive-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Relationship Intelligence
- CRM
- Data Automation
- Contact Management
- Data Quality
- Professional Services
- Sales
- Enrichment
---
