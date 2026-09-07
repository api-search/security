---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Yello Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Yello secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Yello
provider_slug: yello
scheme_count: 1
schemes:
- applies_to: https://www.wayup.com/mcp
  code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://www.wayup.com/api/v1/oauth/o/authorize/
    flow: authorizationCode
    scopes:
      mcp: Access to the WayUp Model Context Protocol server
    tokenUrl: https://www.wayup.com/api/v1/oauth/o/token/
  grant_types_supported:
  - authorization_code
  - refresh_token
  introspection_endpoint: https://www.wayup.com/api/v1/oauth/o/introspect/
  issuer: https://www.wayup.com
  jwks_uri: https://www.wayup.com/api/v1/oauth/o/jwk/
  name: wayup-mcp-oauth
  registration_endpoint: https://www.wayup.com/api/v1/oauth/o/register/
  response_types_supported:
  - code
  revocation_endpoint: https://www.wayup.com/api/v1/oauth/o/revoke-token/
  sources:
  - well-known/yello-wayup-oauth-authorization-server.json
  - well-known/yello-wayup-oauth-protected-resource.json
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: yello-authentication
source_filename: yello-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://www.wayup.com/.well-known/oauth-authorization-server\nnote: >-\n  No OpenAPI exists in this repo, so this profile is not derived from securitySchemes. It is read\n  verbatim from the RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata\n  that www.wayup.com serves for its MCP endpoint. Yello Enterprise tenant sites (customer.yello.co /\n  customer.recsolu.com) are not covered - their authentication model is not publicly documented.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  bearer_methods:\n  - header\n  dynamic_client_registration: true\n  pkce_required_methods:\n  - S256\nschemes:\n- name: wayup-mcp-oauth\n  type: oauth2\n  applies_to: https://www.wayup.com/mcp\n  issuer: https://www.wayup.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.wayup.com/api/v1/oauth/o/authorize/\n    tokenUrl: https://www.wayup.com/api/v1/oauth/o/token/\n\
  \    scopes:\n      mcp: Access to the WayUp Model Context Protocol server\n  registration_endpoint: https://www.wayup.com/api/v1/oauth/o/register/\n  jwks_uri: https://www.wayup.com/api/v1/oauth/o/jwk/\n  revocation_endpoint: https://www.wayup.com/api/v1/oauth/o/revoke-token/\n  introspection_endpoint: https://www.wayup.com/api/v1/oauth/o/introspect/\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - none\n  sources:\n  - well-known/yello-wayup-oauth-authorization-server.json\n  - well-known/yello-wayup-oauth-protected-resource.json\nchallenge:\n  observed_on: https://www.wayup.com/mcp\n  http_status: 401\n  www_authenticate: Bearer resource_metadata=\"https://www.wayup.com/mcp/.well-known/oauth-protected-resource\"\n  spec: RFC 9728 (OAuth 2.0 Protected Resource Metadata)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yello/refs/heads/main/authentication/yello-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Talent Acquisition
- Recruiting
- Human Resources
- Campus Recruiting
- Applicant Tracking
- Recruitment CRM
- Interview Scheduling
- Jobs
- Model Context Protocol
- Government
---
