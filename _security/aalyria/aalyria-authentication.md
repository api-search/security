---
api_key_in: []
auth_types:
- jwt-bearer
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Aalyria Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aalyria secures its APIs with jwt-bearer and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Aalyria
provider_slug: aalyria
scheme_count: 3
schemes:
- algorithm: RS256
  audience_note: The audience is per-RPC — it binds the token to a single gRPC service and method, e.g. https://version.$DOMAIN/aalyria.spacetime.api.version.v1.VersionService/GetVersion
  credential_issuance: Out of band. Public certificate (.crt) is shared with Aalyria; the private key (.key) never leaves the client.
  default: true
  description: The primary Spacetime authentication strategy. The client generates an RSA keypair locally (via `nbictl generate-keys` or OpenSSL), submits the self-signed x509 certificate carrying the public key to Aalyria, and receives a USER_ID, KEY_ID and DOMAIN. Each call is authenticated with a short-lived JWT the client signs itself with the private key and passes as a bearer token in the Authorization header.
  header_claims:
    alg: RS256
    kid: $KEY_ID
    typ: JWT
  name: SelfSignedJWT
  payload_claims:
    aud: https://${DOMAIN}/${GRPC_SERVICE}/${GRPC_METHOD}
    exp: UNIX timestamp
    iat: UNIX timestamp
    iss: $USER_ID
    sub: $USER_ID
  source: https://docs.spacetime.aalyria.com/api/authentication/
  type: jwt-bearer
- default: false
  description: nbictl exposes an `oidc` auth strategy alongside `jwt`, configured with a client id and a token endpoint URL, for Spacetime deployments fronted by an OpenID Connect provider. The issuer/token endpoint is deployment-specific and is not published.
  name: OIDC
  parameters:
  - --auth_strategy=oidc
  - --client_id
  - --token_url
  source: https://github.com/aalyria/api/blob/main/tools/nbictl/README.md
  type: openIdConnect
- default: false
  description: '`--auth_strategy=none` sends no credentials. Intended for local or test Spacetime instances only.'
  name: None
  source: https://github.com/aalyria/api/blob/main/tools/nbictl/README.md
  type: none
slug: aalyria-authentication
source_filename: aalyria-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://docs.spacetime.aalyria.com/api/authentication/\ndocs: https://docs.spacetime.aalyria.com/api/authentication/\nnote: 'Spacetime publishes no OpenAPI, so this profile is not derived from securitySchemes.\n  It is transcribed from the published authentication guide and from the nbictl\n  configuration surface in github.com/aalyria/api (tools/nbictl).'\nsummary:\n  types:\n  - jwt-bearer\n  - openIdConnect\n  transport: gRPC over TLS (HTTP/2); bearer token in the Authorization metadata header\n  oauth2_flows: []\n  api_key_in: []\nschemes:\n- name: SelfSignedJWT\n  type: jwt-bearer\n  default: true\n  description: 'The primary Spacetime authentication strategy. The client generates\n    an RSA keypair locally (via `nbictl generate-keys` or OpenSSL), submits the self-signed\n    x509 certificate carrying the public key to Aalyria, and receives a USER_ID, KEY_ID\n    and DOMAIN. Each call is authenticated with a short-lived\
  \ JWT the client signs\n    itself with the private key and passes as a bearer token in the Authorization\n    header.'\n  algorithm: RS256\n  header_claims:\n    alg: RS256\n    kid: $KEY_ID\n    typ: JWT\n  payload_claims:\n    iss: $USER_ID\n    sub: $USER_ID\n    aud: https://${DOMAIN}/${GRPC_SERVICE}/${GRPC_METHOD}\n    exp: UNIX timestamp\n    iat: UNIX timestamp\n  audience_note: 'The audience is per-RPC — it binds the token to a single gRPC service\n    and method, e.g. https://version.$DOMAIN/aalyria.spacetime.api.version.v1.VersionService/GetVersion'\n  credential_issuance: 'Out of band. Public certificate (.crt) is shared with Aalyria;\n    the private key (.key) never leaves the client.'\n  source: https://docs.spacetime.aalyria.com/api/authentication/\n- name: OIDC\n  type: openIdConnect\n  default: false\n  description: 'nbictl exposes an `oidc` auth strategy alongside `jwt`, configured\n    with a client id and a token endpoint URL, for Spacetime deployments fronted by\n\
  \    an OpenID Connect provider. The issuer/token endpoint is deployment-specific and\n    is not published.'\n  parameters:\n  - --auth_strategy=oidc\n  - --client_id\n  - --token_url\n  source: https://github.com/aalyria/api/blob/main/tools/nbictl/README.md\n- name: None\n  type: none\n  default: false\n  description: '`--auth_strategy=none` sends no credentials. Intended for local or\n    test Spacetime instances only.'\n  source: https://github.com/aalyria/api/blob/main/tools/nbictl/README.md\nauthorization:\n  model: 'Server-side authorization is a first-class API of its own. The Permissions\n    service (aalyria.spacetime.api.permissions.v1alpha) exposes CheckPermission, CheckPermissions,\n    UpdateAuthorizationConfig and ListAuthorizationConfigRevisions, so the authorization\n    configuration is versioned and queryable rather than expressed as OAuth scopes.'\n  source: grpc/api/permissions/v1alpha/permissions.proto\n  oauth_scopes: false\n  scopes_note: 'No OAuth2 authorization\
  \ server and no scope vocabulary are published,\n    so scopes/ is intentionally not emitted for this provider.'\naudit:\n  service: aalyria.spacetime.api.audit.v1alpha.AuditLogService\n  source: grpc/api/audit/v1alpha/audit_logs.proto\ntransport_security:\n  values:\n  - system_cert_pool\n  - insecure\n  default: system_cert_pool\n  transports:\n  - tcp\n  - quic\n  source: https://github.com/aalyria/api/blob/main/tools/nbictl/README.md\nx-evidence:\n- fetched: '2026-08-02'\n  url: https://docs.spacetime.aalyria.com/api/authentication/\n  http_status: 200\n- fetched: '2026-08-02'\n  url: https://github.com/aalyria/api\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aalyria/refs/heads/main/authentication/aalyria-authentication.yml
summary_line: jwt-bearer/openIdConnect · 3 schemes
tags:
- Company
- Networking
- Satellite
- Space
- Telecommunications
- Software Defined Networking
- Orchestration
- Aerospace
- Defense
- Connectivity
- gRPC
- Protocol Buffers
- Telemetry
- Optical Communications
---
