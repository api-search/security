---
anonymous_access: false
api_key_in: []
api_specs:
- filename: developerportal
  format: yaml
  label: Hexagon Nexus API
  slug: nexus-api
  spec_type: OpenAPI
  url: https://nexus.hexagon.com/developerportal
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Hexagon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hexagon declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hexagon
provider_slug: hexagon
scheme_count: 2
schemes:
- applies_to: hexagon-ab:geocloud-graphql
  claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - auth_time
  - name
  - given_name
  - family_name
  - preferred_username
  - email
  - acr
  - azp
  - nonce
  client_id_observed: hxdr_sso
  client_id_source: Read from the public OIDC_CLIENT_ID field of the HxDR single-page application's inline runtime config at https://hxdr.app/ - a public client identifier, not a credential.
  code_challenge_methods_supported:
  - plain
  - S256
  discovery: https://hxauth.com/auth/realms/geo-hxdr-prod/.well-known/openid-configuration
  endpoints:
    authorization: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/auth
    device_authorization: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/auth/device
    dynamic_client_registration: https://hxauth.com/auth/realms/geo-hxdr-prod/clients-registrations/openid-connect
    end_session: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/logout
    introspection: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/token/introspect
    jwks: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/certs
    revocation: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/revoke
    token: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/token
    userinfo: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/userinfo
  format: jwt
  grant_types_supported:
  - authorization_code
  - client_credentials
  - implicit
  - password
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:uma-ticket
  - urn:openid:params:grant-type:ciba
  header: Authorization
  id: hxdr-oidc
  id_token_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - PS256
  - PS384
  - PS512
  - ES256
  - ES384
  - ES512
  - EdDSA
  - HS256
  - HS384
  - HS512
  in: header
  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod
  logout:
    backchannel_logout_supported: true
    frontchannel_logout_supported: true
  machine_to_machine: client_credentials is advertised by the realm, and the realm carries a dedicated service_account scope and an hxdr_be_system_user scope, so a non-interactive integration path exists. Issuance of such a client is not self-service from any public page found in this pass.
  prefix: Bearer
  provider: Keycloak
  realm: geo-hxdr-prod
  scheme: bearer
  token_endpoint_auth_methods_supported:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  type: openIdConnect
  unauthenticated_behaviour:
    graphql_error_code: UNAUTHENTICATED
    http_status: 200
    message: You can not access the requested resource.
    note: GraphQL-idiomatic - transport stays 200 and the failure is carried in errors[].extensions.code. Schema introspection itself is NOT gated and succeeds anonymously.
    probe: POST https://hxdr.app/graphql {"query":"{getUser{id}}"} with no Authorization header
- applies_to: hexagon-ab:geocloud-mcp
  client_registration: 'No registration_endpoint is advertised. The server sets client_id_metadata_document_supported: true, so a client presents a client-ID metadata document URL instead of pre-registering.'
  code_challenge_methods_supported:
  - S256
  discovery: https://geocloud.hexagon.com/.well-known/oauth-authorization-server
  endpoints:
    authorization: https://geocloud.hexagon.com/oauth/authorize
    revocation: https://geocloud.hexagon.com/oauth/revoke
    token: https://geocloud.hexagon.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  header: Authorization
  id: geocloud-mcp-oauth
  in: header
  issuer: https://geocloud.hexagon.com
  prefix: Bearer
  protected_resource_metadata: https://geocloud.hexagon.com/.well-known/oauth-protected-resource
  response_types_supported:
  - code
  scheme: bearer
  scopes_supported:
  - mcp
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
  unauthenticated_behaviour:
    http_status: 401
    message: MCP authentication required.
    probe: POST https://geocloud.hexagon.com/wp-json/mcp/mcp-oauth-server {"jsonrpc":"2.0","id":1,"method":"tools/list"}
slug: hexagon-authentication
source_filename: hexagon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: >-\n  https://hxauth.com/auth/realms/geo-hxdr-prod/.well-known/openid-configuration\n  (HTTP 200, saved verbatim to\n  well-known/hexagon-ab-hxauth-openid-configuration.json);\n  https://geocloud.hexagon.com/.well-known/oauth-authorization-server (HTTP 200);\n  https://geocloud.hexagon.com/.well-known/oauth-protected-resource (HTTP 200);\n  plus live anonymous calls to https://hxdr.app/graphql.\ndocs: https://geocloud.hexagon.com/security-compliance/\nsummary: >-\n  Two separate, unrelated authorization surfaces. The GeoCloud product API is\n  protected by a Keycloak OpenID Connect realm on a dedicated identity host\n  (hxauth.com); the GeoCloud web property's MCP endpoint is protected by a small\n  self-hosted OAuth 2.1 server on geocloud.hexagon.com. They share no issuer, no\n  scopes and no token format.\nschemes:\n  - id: hxdr-oidc\n    applies_to: hexagon-ab:geocloud-graphql\n    type: openIdConnect\n    scheme: bearer\n\
  \    format: jwt\n    in: header\n    header: Authorization\n    prefix: Bearer\n    discovery: https://hxauth.com/auth/realms/geo-hxdr-prod/.well-known/openid-configuration\n    issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n    provider: Keycloak\n    realm: geo-hxdr-prod\n    client_id_observed: hxdr_sso\n    client_id_source: >-\n      Read from the public OIDC_CLIENT_ID field of the HxDR single-page\n      application's inline runtime config at https://hxdr.app/ - a public client\n      identifier, not a credential.\n    endpoints:\n      authorization: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/auth\n      token: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/token\n      userinfo: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/userinfo\n      jwks: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/certs\n      introspection: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/token/introspect\n\
  \      revocation: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/revoke\n      end_session: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/logout\n      device_authorization: https://hxauth.com/auth/realms/geo-hxdr-prod/protocol/openid-connect/auth/device\n      dynamic_client_registration: https://hxauth.com/auth/realms/geo-hxdr-prod/clients-registrations/openid-connect\n    grant_types_supported:\n      - authorization_code\n      - client_credentials\n      - implicit\n      - password\n      - refresh_token\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n      - urn:ietf:params:oauth:grant-type:token-exchange\n      - urn:ietf:params:oauth:grant-type:uma-ticket\n      - urn:openid:params:grant-type:ciba\n    code_challenge_methods_supported:\n      - plain\n      - S256\n    token_endpoint_auth_methods_supported:\n      - private_key_jwt\n      - client_secret_basic\n      - client_secret_post\n\
  \      - tls_client_auth\n      - client_secret_jwt\n    id_token_signing_alg_values_supported:\n      - RS256\n      - RS384\n      - RS512\n      - PS256\n      - PS384\n      - PS512\n      - ES256\n      - ES384\n      - ES512\n      - EdDSA\n      - HS256\n      - HS384\n      - HS512\n    claims_supported:\n      - iss\n      - sub\n      - aud\n      - exp\n      - iat\n      - auth_time\n      - name\n      - given_name\n      - family_name\n      - preferred_username\n      - email\n      - acr\n      - azp\n      - nonce\n    logout:\n      backchannel_logout_supported: true\n      frontchannel_logout_supported: true\n    machine_to_machine: >-\n      client_credentials is advertised by the realm, and the realm carries a\n      dedicated service_account scope and an hxdr_be_system_user scope, so a\n      non-interactive integration path exists. Issuance of such a client is not\n      self-service from any public page found in this pass.\n    unauthenticated_behaviour:\n     \
  \ probe: 'POST https://hxdr.app/graphql {\"query\":\"{getUser{id}}\"} with no Authorization header'\n      http_status: 200\n      graphql_error_code: UNAUTHENTICATED\n      message: You can not access the requested resource.\n      note: >-\n        GraphQL-idiomatic - transport stays 200 and the failure is carried in\n        errors[].extensions.code. Schema introspection itself is NOT gated and\n        succeeds anonymously.\n  - id: geocloud-mcp-oauth\n    applies_to: hexagon-ab:geocloud-mcp\n    type: oauth2\n    scheme: bearer\n    in: header\n    header: Authorization\n    prefix: Bearer\n    discovery: https://geocloud.hexagon.com/.well-known/oauth-authorization-server\n    protected_resource_metadata: https://geocloud.hexagon.com/.well-known/oauth-protected-resource\n    issuer: https://geocloud.hexagon.com\n    endpoints:\n      authorization: https://geocloud.hexagon.com/oauth/authorize\n      token: https://geocloud.hexagon.com/oauth/token\n      revocation: https://geocloud.hexagon.com/oauth/revoke\n\
  \    grant_types_supported:\n      - authorization_code\n      - refresh_token\n    response_types_supported:\n      - code\n    code_challenge_methods_supported:\n      - S256\n    token_endpoint_auth_methods_supported:\n      - none\n    scopes_supported:\n      - mcp\n    client_registration: >-\n      No registration_endpoint is advertised. The server sets\n      client_id_metadata_document_supported: true, so a client presents a\n      client-ID metadata document URL instead of pre-registering.\n    unauthenticated_behaviour:\n      probe: 'POST https://geocloud.hexagon.com/wp-json/mcp/mcp-oauth-server {\"jsonrpc\":\"2.0\",\"id\":1,\"method\":\"tools/list\"}'\n      http_status: 401\n      message: MCP authentication required.\ngaps:\n  - >-\n    No public developer-facing authentication guide was found for the GeoCloud\n    GraphQL API. Everything recorded here was read from discovery documents and\n    live probes, not from a documentation page.\n  - >-\n    No API-key or personal-access-token\
  \ mechanism exists in either surface; every\n    call requires an OAuth/OIDC bearer token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hexagon/refs/heads/main/authentication/hexagon-authentication.yml
summary_line: 2 schemes
tags:
- Manufacturing
- Metrology
- Quality Inspection
- Digital Factory
- Production Monitoring
- Industrial IoT
- Smart Manufacturing
---
