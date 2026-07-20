---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Legitfit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: LegitFit secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: LegitFit
provider_slug: legitfit
scheme_count: 1
schemes:
- client_id_metadata_document_supported: true
  flows:
  - authorizationUrl: https://legitfit.com/api/oauth2/authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    response_types_supported:
    - code
    scopes:
    - mcp:read
    - mcp:write
    tokenUrl: https://legitfit.com/api/oauth2/token
  issuer: https://legitfit.com
  name: LegitFitOAuth2
  sources:
  - well-known/legitfit-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: legitfit-authentication
source_filename: legitfit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://legitfit.com/.well-known/oauth-authorization-server\ndocs: https://legitfit.com/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  bearer_methods:\n  - header\n  pkce_required_methods:\n  - S256\nnote: >-\n  Derived from LegitFit's published RFC 8414 authorization-server metadata and RFC 9728\n  protected-resource metadata rather than from an OpenAPI document — LegitFit publishes\n  no public OpenAPI. The only publicly advertised protected resource is the MCP server\n  at https://legitfit.com/api/mcp. LegitFit does not publish an OpenID Connect discovery\n  document, so this is plain OAuth 2.x/2.1 authorization, not OIDC.\nschemes:\n- name: LegitFitOAuth2\n  type: oauth2\n  issuer: https://legitfit.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://legitfit.com/api/oauth2/authorize\n    tokenUrl: https://legitfit.com/api/oauth2/token\n\
  \    response_types_supported:\n    - code\n    code_challenge_methods_supported:\n    - S256\n    scopes:\n    - mcp:read\n    - mcp:write\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  client_id_metadata_document_supported: true\n  sources:\n  - well-known/legitfit-oauth-authorization-server.json\nprotected_resources:\n- resource: https://legitfit.com/api/mcp\n  bearer_methods_supported:\n  - header\n  scopes_supported:\n  - mcp:read\n  - mcp:write\n  source: well-known/legitfit-oauth-protected-resource.json\nend_user_login: https://legitfit.com/authenticate/signin\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legitfit/refs/heads/main/authentication/legitfit-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fitness
- Gym Management
- Studio Management
- Scheduling
- Memberships
- Payments
- SaaS
- MCP
- Ireland
---
