---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Liftlab Authentication
name_suffix: Authentication
oauth_flows: []
overview: LiftLab declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LiftLab
provider_slug: liftlab
scheme_count: 1
schemes:
- bearer_methods:
  - header
  description: OAuth 2.0 protecting the LiftLab Connect MCP endpoint https://connect.liftlab.com/server/api/mcp. Advertised via RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata.
  dynamic_client_registration:
    note: No registration_endpoint is present in the authorization-server metadata, and /.well-known/openid-configuration returns 404, so clients cannot self-register — a client must be provisioned by LiftLab/TapClicks.
    supported: false
  flows:
  - authorization_url: https://connect.liftlab.com/server/api/mcp/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    pkce: required-advertised
    refresh_supported: true
    scopes:
      claudeai: The only scope the authorization server advertises. Named for the Claude connector integration this MCP server is deployed for. LiftLab publishes no scope reference page, so no description beyond the scope string itself is available.
    token_url: https://connect.liftlab.com/server/api/mcp/token
  - flow: clientCredentials
    scopes:
      claudeai: Same single advertised scope.
    token_url: https://connect.liftlab.com/server/api/mcp/token
  issuer: https://connect.liftlab.com
  name: oauth2
  response_types:
  - code
  revocation_endpoint: https://connect.liftlab.com/server/api/oauth/revoke
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  type: oauth2
slug: liftlab-authentication
source_filename: liftlab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://connect.liftlab.com/.well-known/oauth-authorization-server +\n  https://connect.liftlab.com/.well-known/oauth-protected-resource +\n  live 401 challenge from https://connect.liftlab.com/server/api/mcp\nnote: >-\n  Derived entirely from the two RFC 8414 / RFC 9728 discovery documents LiftLab\n  serves at connect.liftlab.com and from the live WWW-Authenticate challenge.\n  LiftLab publishes no developer documentation and no OpenAPI, so there is no\n  docs page to upgrade this from — every value below was read off a machine\n  document, not prose.\n\nschemes:\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 protecting the LiftLab Connect MCP endpoint\n    https://connect.liftlab.com/server/api/mcp. Advertised via RFC 8414\n    authorization-server metadata and RFC 9728 protected-resource metadata.\n  issuer: https://connect.liftlab.com\n  flows:\n  - flow: authorizationCode\n    authorization_url:\
  \ https://connect.liftlab.com/server/api/mcp/authorize\n    token_url: https://connect.liftlab.com/server/api/mcp/token\n    refresh_supported: true\n    pkce: required-advertised\n    code_challenge_methods:\n    - S256\n    scopes:\n      claudeai: >-\n        The only scope the authorization server advertises. Named for the Claude\n        connector integration this MCP server is deployed for. LiftLab publishes\n        no scope reference page, so no description beyond the scope string itself\n        is available.\n  - flow: clientCredentials\n    token_url: https://connect.liftlab.com/server/api/mcp/token\n    scopes:\n      claudeai: >-\n        Same single advertised scope.\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  response_types:\n  - code\n  bearer_methods:\n  - header\n  revocation_endpoint: https://connect.liftlab.com/server/api/oauth/revoke\n  dynamic_client_registration:\n    supported: false\n    note: >-\n      No registration_endpoint is present\
  \ in the authorization-server metadata,\n      and /.well-known/openid-configuration returns 404, so clients cannot\n      self-register — a client must be provisioned by LiftLab/TapClicks.\n\nsurfaces:\n- surface: MCP\n  url: https://connect.liftlab.com/server/api/mcp\n  auth: oauth2\n  anonymous_status: 401\n  challenge: >-\n    WWW-Authenticate: Bearer resource_metadata=\"https://connect.liftlab.com/.well-known/oauth-protected-resource\"\n  error_envelope: '{\"error\":true,\"data\":[\"Please login to access the API\"],\"warnings\":[],\"status\":401}'\n\nnot_found:\n- path: /.well-known/openid-configuration\n  host: connect.liftlab.com\n  status: 404\n  note: No OpenID Connect discovery; this is plain OAuth 2.0, not OIDC.\n- path: /.well-known/jwks.json\n  host: connect.liftlab.com\n  status: 404\n\nx-evidence:\n- url: https://connect.liftlab.com/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://connect.liftlab.com/.well-known/oauth-protected-resource\n\
  \  http_status: 200\n  fetched: '2026-08-13'\n- url: https://connect.liftlab.com/server/api/mcp\n  http_status: 401\n  fetched: '2026-08-13'\n\nownership_note: >-\n  connect.liftlab.com is LiftLab's own hostname (Let's Encrypt cert\n  CN=connect.liftlab.com) running a white-labeled TapClicks portal (CNAME to\n  liftlabtrial.tapclicks.com); the OAuth issuer is https://connect.liftlab.com.\n  See mcp/liftlab-mcp.yml for the full ownership finding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liftlab/refs/heads/main/authentication/liftlab-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Enterprise
- Marketing
- Marketing Measurement
- Marketing Mix Modeling
- Incrementality
- Analytics
- Martech
- Attribution
- Budget Optimization
- Data Science
- Software-as-a-Service
---
