---
api_key_in: []
auth_types: []
description: Laurence's only publicly documented programmatic surface is its hosted MCP server, which is an OAuth 2.0 protected resource. The authorization server is www.laurence.com; the protected resource is the MCP endpoint on modal.run. The flow is authorization code with PKCE (S256 only) and supports OAuth 2.0 Dynamic Client Registration — token_endpoint_auth_methods_supported is "none", i.e. public clients only, which is what lets an IDE register itself and complete a browser sign-in without any pre-issued credential. There is no documented API-key or HTTP-basic surface, and no general-purpose REST API is published.
kind: authentication
layout: security
method: searched
name: Laurence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Laurence declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Laurence
provider_slug: laurence
scheme_count: 1
schemes:
- applies_to:
  - https://laurence-ai-68564--ask-laurence-agent-mcp-server.modal.run/mcp
  authorization_url: https://www.laurence.com/api/mcp/oauth/authorize
  bearer_methods:
  - header
  client_registration: dynamic
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://www.laurence.com
  jwks_status: 503
  jwks_uri: https://www.laurence.com/.well-known/jwks.json
  name: laurence_mcp_oauth
  pkce:
    code_challenge_methods:
    - S256
    required: true
  registration_url: https://www.laurence.com/api/mcp/oauth/register
  response_types:
  - code
  scopes:
  - openid
  - profile
  - email
  - laurence:mcp
  subject_types:
  - public
  token_endpoint_auth_methods:
  - none
  token_url: https://www.laurence.com/api/mcp/oauth/token
  type: oauth2
slug: laurence-authentication
source_filename: laurence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://www.laurence.com/.well-known/openid-configuration,\n  https://www.laurence.com/.well-known/oauth-authorization-server,\n  https://laurence-ai-68564--ask-laurence-agent-mcp-server.modal.run/.well-known/oauth-protected-resource,\n  https://www.laurence.com/blog/laurence-mcp-launch\ndocs: https://www.laurence.com/blog/laurence-mcp-launch\ndescription: >-\n  Laurence's only publicly documented programmatic surface is its hosted MCP server, which is an\n  OAuth 2.0 protected resource. The authorization server is www.laurence.com; the protected resource\n  is the MCP endpoint on modal.run. The flow is authorization code with PKCE (S256 only) and\n  supports OAuth 2.0 Dynamic Client Registration — token_endpoint_auth_methods_supported is \"none\",\n  i.e. public clients only, which is what lets an IDE register itself and complete a browser sign-in\n  without any pre-issued credential. There is no documented API-key or\
  \ HTTP-basic surface, and no\n  general-purpose REST API is published.\nschemes:\n  - name: laurence_mcp_oauth\n    type: oauth2\n    flow: authorizationCode\n    issuer: https://www.laurence.com\n    authorization_url: https://www.laurence.com/api/mcp/oauth/authorize\n    token_url: https://www.laurence.com/api/mcp/oauth/token\n    registration_url: https://www.laurence.com/api/mcp/oauth/register\n    jwks_uri: https://www.laurence.com/.well-known/jwks.json\n    jwks_status: 503\n    pkce:\n      required: true\n      code_challenge_methods:\n        - S256\n    grant_types:\n      - authorization_code\n      - refresh_token\n    response_types:\n      - code\n    token_endpoint_auth_methods:\n      - none\n    client_registration: dynamic\n    subject_types:\n      - public\n    bearer_methods:\n      - header\n    scopes:\n      - openid\n      - profile\n      - email\n      - laurence:mcp\n    applies_to:\n      - https://laurence-ai-68564--ask-laurence-agent-mcp-server.modal.run/mcp\n\
  authorization_model:\n  tenancy: >-\n    Every tool call is scoped to the Amazon Ads profiles the signed-in user belongs to. Callers pass\n    a profile_id and the server returns only data that user is permitted to see.\n  discovery_tool: list_allowed_ads_profiles\n  access: Laurence customers only\n  read_only: true\nobserved:\n  probed: '2026-07-19'\n  unauthenticated_request_status: 401\n  challenge: >-\n    WWW-Authenticate: Bearer error=\"invalid_token\", error_description=\"Authentication required\",\n    resource_metadata=\"https://laurence-ai-68564--ask-laurence-agent-mcp-server.modal.run/.well-known/oauth-protected-resource/mcp\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laurence/refs/heads/main/authentication/laurence-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Advertising
- Amazon
- E-Commerce
- Marketing
- Machine Learning
- Retail Media
- MCP
---
