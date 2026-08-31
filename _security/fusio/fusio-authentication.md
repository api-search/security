---
api_key_in: []
api_specs:
- filename: fusio-backend.json
  format: json
  label: Fusio Backend API
  slug: fusio-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusio/refs/heads/main/openapi/fusio-backend.json
- filename: fusio-consumer.json
  format: json
  label: Fusio Consumer API
  slug: fusio-consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusio/refs/heads/main/openapi/fusio-consumer.json
- filename: fusio-system.json
  format: json
  label: Fusio System API
  slug: fusio-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusio/refs/heads/main/openapi/fusio-system.json
- filename: fusio-authorization.json
  format: json
  label: Fusio Authorization API
  slug: fusio-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusio/refs/heads/main/openapi/fusio-authorization.json
auth_types:
- oauth2
description: Fusio ships its own OAuth2 authorization server (added in 6.0.0) rather than delegating to one, and publishes RFC 8414, RFC 9728 and OpenID Connect discovery documents from every instance. The single securityScheme in the generated contracts is thin - it advertises only the 'default' scope because the generator emits what the anonymous caller can see - so the real model below is read from the docs and the discovery documents, not from the spec alone.
kind: authentication
layout: security
method: searched
name: Fusio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Fusio secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Fusio
provider_slug: fusio
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://demo.fusio-project.org/authorization/token
  - authorizationUrl: https://demo.fusio-project.org/authorization/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://demo.fusio-project.org/authorization/token
  name: app
  sources:
  - openapi/fusio-authorization.json
  - openapi/fusio-backend.json
  - openapi/fusio-consumer.json
  - openapi/fusio-system.json
  type: oauth2
slug: fusio-authentication
source_filename: fusio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: openapi/fusio-authorization.json, openapi/fusio-backend.json, openapi/fusio-consumer.json, openapi/fusio-system.json;\n  enriched from https://docs.fusio-project.org/docs/security/authentication, https://docs.fusio-project.org/docs/security/authorization,\n  https://docs.fusio-project.org/docs/security/personal_access_token and https://demo.fusio-project.org/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: app\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://demo.fusio-project.org/authorization/token\n    scopes: 2\n  - flow: authorizationCode\n    authorizationUrl: https://demo.fusio-project.org/authorization/authorize\n    tokenUrl: https://demo.fusio-project.org/authorization/token\n    scopes: 2\n  sources:\n  - openapi/fusio-authorization.json\n  - openapi/fusio-backend.json\n  - openapi/fusio-consumer.json\n\
  \  - openapi/fusio-system.json\ndocs: https://docs.fusio-project.org/docs/security/authentication\nprovider: Fusio\nproviderId: fusio\ndescription: Fusio ships its own OAuth2 authorization server (added in 6.0.0) rather than delegating to\n  one, and publishes RFC 8414, RFC 9728 and OpenID Connect discovery documents from every instance. The\n  single securityScheme in the generated contracts is thin - it advertises only the 'default' scope because\n  the generator emits what the anonymous caller can see - so the real model below is read from the docs\n  and the discovery documents, not from the spec alone.\nmethods:\n- name: OAuth2 authorization server\n  endpoint: /authorization/token\n  grants:\n  - authorization_code\n  - client_credentials\n  - password\n  - refresh_token\n  authorization_endpoint: /authorization/authorize\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  signing_alg: HS256\n  docs: https://docs.fusio-project.org/docs/security/authorization\n  note: The\
  \ full path. Client id and secret come from an app created in the backend; every redirect URI\n    must share the app URL base.\n- name: Simple login\n  endpoint: /consumer/login\n  http: POST\n  payload: '{\"username\": \"...\", \"password\": \"...\"}'\n  returns: a JWT access token\n  refresh: PUT /consumer/login\n  docs: https://docs.fusio-project.org/docs/security/authentication\n  note: The shortest path to a token, intended for an operator’s own SPA.\n- name: Personal access token\n  endpoint: /consumer/token\n  http: POST\n  operationId: consumer.token.create\n  scoped: true\n  docs: https://docs.fusio-project.org/docs/security/personal_access_token\n  note: GitHub-style manually created token with a chosen subset of scopes. The right choice for machine-to-machine\n    use.\n- name: External OIDC identity provider\n  endpoint: /consumer/identity\n  docs: https://docs.fusio-project.org/docs/security/authentication\n  note: Fusio is also an OIDC relying party. Identity providers such\
  \ as Keycloak, Entra ID or Okta are\n    configured under System / Identity and bound to an app; the callback returns access_token, token_type,\n    expires_in, refresh_token and scope as query parameters on the app redirect_uri.\ntoken:\n  transport: 'Authorization: Bearer <token>'\n  bearer_methods_supported:\n  - header\n  expiry: instance-configurable; every token expires\n  refresh: refresh_token grant or PUT /consumer/login\n  revocation: POST /authorization/revoke (self), DELETE /backend/app/{app_id}/token/{token_id} (operator),\n    DELETE /consumer/token/{token_id} (consumer)\n  introspection: GET /authorization/whoami returns the identity a token resolves to\ndiscovery:\n  oauth_authorization_server: well-known/fusio-oauth-authorization-server.json\n  oauth_protected_resource: well-known/fusio-oauth-protected-resource.json\n  openid_configuration: well-known/fusio-openid-configuration.json\n  claims_supported:\n  - iss\n  - sub\n  - iat\n  - exp\n  - name\n  - preferred_username\n\
  \  - aud\n  - email\nscopes_detail: scopes/fusio-scopes.yml\nspec_gap: The harvested contracts declare the oauth2 scheme with only the 'default' scope, because the\n  OpenAPI is generated live for the anonymous caller. The instance actually defines 58 scopes, recovered\n  from the filtered per-category specs and recorded in scopes/fusio-scopes.yml.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fusio/refs/heads/main/authentication/fusio-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- API Management
- Open-Source
- REST API
- API Gateway
- Developer Portal
- OpenAPI
- Self-Hosted
- MCP
---
