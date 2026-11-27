---
anonymous_access: false
api_key_in: []
api_specs:
- filename: codeatlas-com-br-contact-api-openapi.yml
  format: yaml
  label: CodeAtlas Contact API
  slug: codeatlas-com-br-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeatlas-com-br/openapi/codeatlas-com-br-contact-api-openapi.yml
- filename: codeatlas-com-br-discovery-api-openapi.yml
  format: yaml
  label: CodeAtlas Discovery API
  slug: codeatlas-com-br-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeatlas-com-br/openapi/codeatlas-com-br-discovery-api-openapi.yml
- filename: codeatlas-com-br-exports-api-openapi.yml
  format: yaml
  label: CodeAtlas Exports API
  slug: codeatlas-com-br-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeatlas-com-br/openapi/codeatlas-com-br-exports-api-openapi.yml
- filename: codeatlas-com-br-oauth-api-openapi.yml
  format: yaml
  label: CodeAtlas OAuth API
  slug: codeatlas-com-br-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeatlas-com-br/openapi/codeatlas-com-br-oauth-api-openapi.yml
- filename: codeatlas-com-br-system-api-openapi.yml
  format: yaml
  label: CodeAtlas System API
  slug: codeatlas-com-br-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeatlas-com-br/openapi/codeatlas-com-br-system-api-openapi.yml
auth_types:
- none
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CodeAtlas Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- urn:workos:agent-auth:grant-type:claim
overview: CodeAtlas secures its APIs with none and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and urn:workos:agent-auth:grant-type:claim flow(s).
provider_name: CodeAtlas
provider_slug: codeatlas-com-br
scheme_count: 2
schemes:
- description: OAuth 2.0 client_credentials after dynamic client registration (RFC 7591) at POST /oauth2/register. Access token is an HS256 JWT (iss, sub, aud, scope, iat, exp, jti) valid 3600 seconds; no refresh_token. client_secret_basic or client_secret_post.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://codeatlas.com.br/oauth2/token
  name: oauth2ClientCredentials
  sources:
  - openapi/codeatlas-com-br-openapi.yml
  - https://codeatlas.com.br/auth.md
  type: oauth2
- description: Agent registration from the person's email via POST /agent/identity, confirmed with a 6-digit code in a claim ceremony (600 second window, poll interval 5 seconds). Documented in auth.md; not declared as a securityScheme in the OpenAPI.
  flows:
  - flow: urn:workos:agent-auth:grant-type:claim
    tokenUrl: https://codeatlas.com.br/oauth2/token
  name: service_auth
  sources:
  - https://codeatlas.com.br/auth.md
  type: oauth2
slug: codeatlas-com-br-authentication
source_filename: codeatlas-com-br-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://codeatlas.com.br/auth.md\ndocs: https://codeatlas.com.br/auth.md\nsummary:\n  types:\n  - none\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - urn:workos:agent-auth:grant-type:claim\n  note: Read endpoints are public. Write endpoints use OAuth 2.0 Bearer tokens.\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://codeatlas.com.br/oauth2/token\n    scopes: 1\n  description: OAuth 2.0 client_credentials after dynamic client registration (RFC 7591) at POST /oauth2/register.\n    Access token is an HS256 JWT (iss, sub, aud, scope, iat, exp, jti) valid 3600 seconds; no refresh_token. client_secret_basic\n    or client_secret_post.\n  sources:\n  - openapi/codeatlas-com-br-openapi.yml\n  - https://codeatlas.com.br/auth.md\n- name: service_auth\n  type: oauth2\n  flows:\n  - flow: urn:workos:agent-auth:grant-type:claim\n    tokenUrl: https://codeatlas.com.br/oauth2/token\n\
  \  description: Agent registration from the person's email via POST /agent/identity, confirmed with a 6-digit code\n    in a claim ceremony (600 second window, poll interval 5 seconds). Documented in auth.md; not declared as a securityScheme\n    in the OpenAPI.\n  sources:\n  - https://codeatlas.com.br/auth.md\ndiscovery:\n  protected_resource_metadata: https://codeatlas.com.br/.well-known/oauth-protected-resource\n  authorization_server_metadata: https://codeatlas.com.br/.well-known/oauth-authorization-server\n  revocation_endpoint: https://codeatlas.com.br/oauth2/revoke\n  www_authenticate: Bearer resource_metadata=..., scope=\"api:write\"\naudiences:\n- https://codeatlas.com.br/api/v1\n- https://codeatlas.com.br/api/sandbox/v1\n"
source_yaml_url: https://artifacts.apis.io/codeatlas-com-br/authentication/codeatlas-com-br-authentication.yml
summary_line: none/oauth2 · 2 schemes
tags:
- Company
- Software Development
- Developer Tools
- AI Agents
- MCP
- Custom Software
- Brazil
---
