---
api_key_in: []
auth_types: []
description: 'Solve Intelligence protects its public MCP surface with OAuth 2.0 bearer tokens issued by a first-party authorization server it operates at https://api.solveintelligence.com/auth. The deployment is standards-forward: the resource server advertises RFC 9728 protected-resource metadata, returns a conformant RFC 6750 WWW-Authenticate challenge naming both the metadata URL and the required scopes, and the authorization server publishes OpenID Connect discovery metadata. This is discoverable without credentials, which is why this profile can describe the auth model precisely even though the API itself is subscription-gated.'
kind: authentication
layout: security
method: probed
name: Solve Intelligence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Solve Intelligence declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Solve Intelligence
provider_slug: solve-intelligence
scheme_count: 1
schemes:
- applies_to:
  - https://api.solveintelligence.com/mcp/
  bearer_methods_supported:
  - header
  description: Authorization-code flow with a browser sign-in on first connect. MCP clients then reuse the issued credentials for subsequent sessions; the offline_access scope supports refresh.
  flows:
    authorizationCode:
      authorizationUrl: https://api.solveintelligence.com/auth/oauth/auth
      refreshUrl: https://api.solveintelligence.com/auth/oauth/token
      scopes:
        mcp:ask_solve: Call the Solve MCP research surface.
        offline_access: Issue a refresh token so the client can renew access without a new browser sign-in.
      tokenUrl: https://api.solveintelligence.com/auth/oauth/token
  format: Bearer <token>
  header: Authorization
  id: solve_mcp_oauth
  in: header
  scheme_class: OAuth 2.0 / OpenID Connect
  type: oauth2
slug: solve-intelligence-authentication
source_filename: solve-intelligence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: >-\n  https://api.solveintelligence.com/.well-known/oauth-protected-resource (HTTP 200),\n  https://api.solveintelligence.com/auth/.well-known/openid-configuration (HTTP 200), and the\n  WWW-Authenticate challenge returned by https://api.solveintelligence.com/mcp/ (HTTP 401)\nname: Solve Intelligence authentication\ndescription: >-\n  Solve Intelligence protects its public MCP surface with OAuth 2.0 bearer tokens issued by a\n  first-party authorization server it operates at https://api.solveintelligence.com/auth. The\n  deployment is standards-forward: the resource server advertises RFC 9728 protected-resource\n  metadata, returns a conformant RFC 6750 WWW-Authenticate challenge naming both the metadata\n  URL and the required scopes, and the authorization server publishes OpenID Connect discovery\n  metadata. This is discoverable without credentials, which is why this profile can describe the\n  auth model precisely even though\
  \ the API itself is subscription-gated.\n\nschemes:\n  - id: solve_mcp_oauth\n    type: oauth2\n    scheme_class: OAuth 2.0 / OpenID Connect\n    description: >-\n      Authorization-code flow with a browser sign-in on first connect. MCP clients then reuse the\n      issued credentials for subsequent sessions; the offline_access scope supports refresh.\n    flows:\n      authorizationCode:\n        authorizationUrl: https://api.solveintelligence.com/auth/oauth/auth\n        tokenUrl: https://api.solveintelligence.com/auth/oauth/token\n        refreshUrl: https://api.solveintelligence.com/auth/oauth/token\n        scopes:\n          offline_access: Issue a refresh token so the client can renew access without a new\n            browser sign-in.\n          mcp:ask_solve: Call the Solve MCP research surface.\n    bearer_methods_supported:\n      - header\n    in: header\n    header: Authorization\n    format: Bearer <token>\n    applies_to:\n      - https://api.solveintelligence.com/mcp/\n\
  \nauthorization_server:\n  issuer: https://api.solveintelligence.com/auth\n  implementation: >-\n    SuperTokens (identified from the Content-Security-Policy header served by the API host, which\n    allowlists cdn.jsdelivr.net/gh/supertokens/).\n  endpoints:\n    authorization: https://api.solveintelligence.com/auth/oauth/auth\n    token: https://api.solveintelligence.com/auth/oauth/token\n    userinfo: https://api.solveintelligence.com/auth/oauth/userinfo\n    revocation: https://api.solveintelligence.com/auth/oauth/revoke\n    introspection: https://api.solveintelligence.com/auth/oauth/introspect\n    end_session: https://api.solveintelligence.com/auth/oauth/end_session\n    jwks: https://api.solveintelligence.com/auth/jwt/jwks.json\n  subject_types_supported:\n    - public\n  id_token_signing_alg_values_supported:\n    - RS256\n  response_types_supported:\n    - code\n    - id_token\n    - id_token token\n\nchallenge:\n  status: 401\n  www_authenticate: >-\n    Bearer realm=\"mcp\"\
  ,\n    resource_metadata=\"https://api.solveintelligence.com/.well-known/oauth-protected-resource\",\n    scope=\"offline_access mcp:ask_solve\"\n  body: MCP bearer token is required\n  note: >-\n    A conformant RFC 9728 challenge. An MCP client that receives this can discover the\n    authorization server and required scopes with no out-of-band configuration, which is the\n    behaviour the spec asks for and which most gated MCP servers still do not implement.\n\nentitlement:\n  subscription_required: true\n  note: >-\n    An active Solve Intelligence subscription is required, and the provider states that only\n    Solve organization administrators can enable the MCP integration for their users. There is no\n    self-serve developer signup, no API key issuance page, and no public sandbox.\n\nsso:\n  note: >-\n    Not documented on any public page. The security page describes encryption, subprocessor\n    regionality and training exclusions but does not name SSO/SAML/MFA support.\n\n\
  gaps:\n  - The REST OpenAPI at https://api.solveintelligence.com/openapi.json returns HTTP 401, so the\n    full securityScheme set for the underlying REST API could not be read anonymously.\n  - No /.well-known/oauth-authorization-server at the host root; RFC 8414 discovery is only\n    reachable through the OIDC path under the issuer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solve-intelligence/refs/heads/main/authentication/solve-intelligence-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Legal
- Legal Tech
- Intellectual Property
- Patents
- Artificial Intelligence
- Document Generation
- Search
- MCP
- Agents
---
