---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: SiFive has no public REST API with an OpenAPI to derive security schemes from, so this profile is probed directly from the live RFC 8414 Authorization Server Metadata that the SiFive Cloud Services (SCS) portal serves anonymously. Every value below is copied from that document or from a probe of the endpoint it names.
kind: authentication
layout: security
method: probed
name: Sifive Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: SiFive secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: SiFive
provider_slug: sifive
scheme_count: 1
schemes:
- code_challenge_methods:
  - S256
  flows:
  - authorizationUrl: https://scs.sifive.com/o/authorize/
    flow: authorizationCode
    scopes:
    - openid
    - mcp:read
    - mcp:write
    tokenUrl: https://scs.sifive.com/o/token/
  - flow: refreshToken
    tokenUrl: https://scs.sifive.com/o/token/
  id_token_signing_alg:
  - RS256
  issuer_actual: https://scs.sifive.com/o
  issuer_declared: http://localhost:8000/o
  name: SiFiveCloudServicesOAuth2
  response_types:
  - code
  source: https://scs.sifive.com/.well-known/oauth-authorization-server
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
slug: sifive-authentication
source_filename: sifive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://scs.sifive.com/.well-known/oauth-authorization-server\ndocs: https://www.sifive.com/software/sifive-core-designer\ndescription: >-\n  SiFive has no public REST API with an OpenAPI to derive security schemes from, so this\n  profile is probed directly from the live RFC 8414 Authorization Server Metadata that the\n  SiFive Cloud Services (SCS) portal serves anonymously. Every value below is copied from\n  that document or from a probe of the endpoint it names.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken]\n  pkce: [S256]\n  implementation: django-oauth-toolkit\nschemes:\n- name: SiFiveCloudServicesOAuth2\n  type: oauth2\n  source: https://scs.sifive.com/.well-known/oauth-authorization-server\n  issuer_declared: http://localhost:8000/o\n  issuer_actual: https://scs.sifive.com/o\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://scs.sifive.com/o/authorize/\n\
  \    tokenUrl: https://scs.sifive.com/o/token/\n    scopes: [openid, 'mcp:read', 'mcp:write']\n  - flow: refreshToken\n    tokenUrl: https://scs.sifive.com/o/token/\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  code_challenge_methods: [S256]\n  response_types: [code]\n  id_token_signing_alg: [RS256]\n  subject_types: [public]\nendpoints:\n- {name: authorization, url: 'https://scs.sifive.com/o/authorize/', probed_status: 302}\n- {name: token, url: 'https://scs.sifive.com/o/token/', probed_status: 405, note: 'GET rejected; POST only'}\n- {name: registration, url: 'https://scs.sifive.com/o/register/', probed_status: 405, spec: 'RFC 7591 dynamic client registration'}\n- {name: revocation, url: 'https://scs.sifive.com/o/revoke_token/', probed_status: 405, spec: 'RFC 7009'}\n- {name: introspection, url: 'https://scs.sifive.com/o/introspect/', probed_status: 403, spec: 'RFC 7662'}\n- {name: userinfo, url: 'https://scs.sifive.com/o/userinfo/', probed_status:\
  \ 401, spec: 'OIDC Core 1.0'}\n- {name: jwks, url: 'https://scs.sifive.com/o/.well-known/jwks.json', probed_status: 200, note: 'empty key set'}\nobservations:\n- id: issuer-points-at-localhost\n  severity: high\n  finding: >-\n    The production metadata document declares issuer \"http://localhost:8000/o\" and every\n    endpoint URL as \"http://localhost:8000/o/...\". The real, working endpoints are on\n    https://scs.sifive.com/o/. A spec-conformant OAuth client that follows RFC 8414 and\n    RFC 9207 issuer validation cannot use this document as published: it will either\n    refuse the mismatched issuer or attempt cleartext HTTP to a loopback address.\n  evidence: well-known/sifive-oauth-authorization-server.json\n  remedy: >-\n    Set the deployment's OAUTH2_PROVIDER issuer/base URL to https://scs.sifive.com/o so the\n    metadata document reflects the deployed origin.\n- id: empty-jwks\n  severity: medium\n  finding: >-\n    id_token_signing_alg_values_supported declares RS256 but\
  \ the advertised jwks_uri\n    returns {\"keys\": []}, so no relying party can verify a signed ID token from published\n    key material.\n  evidence: well-known/sifive-jwks.json\n- id: no-openid-configuration\n  severity: low\n  finding: >-\n    The \"openid\" scope and RS256 ID-token signing are advertised, but\n    /.well-known/openid-configuration returns 404 — OIDC discovery is not served, only the\n    OAuth 2.0 (RFC 8414) variant.\n- id: token-endpoint-auth-none-allowed\n  severity: informational\n  finding: >-\n    token_endpoint_auth_methods_supported includes \"none\", which is the expected posture\n    for public clients paired with the mandatory-looking S256 PKCE support.\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://scs.sifive.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sifive/refs/heads/main/authentication/sifive-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Semiconductors
- RISC-V
- Processor IP
- Chip Design
- Embedded
- Hardware
- Developer Tools
- Electronic Design Automation
- OAuth
---
