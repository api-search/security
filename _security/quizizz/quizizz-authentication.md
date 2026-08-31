---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Quizizz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wayground declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Wayground
provider_slug: quizizz
scheme_count: 1
schemes:
- applies_to:
  - https://wayground.com/_quizizzmcp/main/mcp
  authorization_url: https://wayground.com/_authserver/public/public/v1/oauth/authorize
  client_authentication:
  - none
  client_type: public
  dynamic_client_registration: true
  flow: authorizationCode
  name: wayground_mcp_oauth
  pkce_methods:
  - S256
  pkce_required: true
  refresh_tokens: true
  registration_url: https://wayground.com/_authserver/public/public/v1/oauth/register
  resource_indicators: true
  revocation_url: https://wayground.com/_authserver/public/public/v1/oauth/revoke
  scopes:
  - description: The single scope Wayground advertises. Verbatim from scopes_supported in both the authorization-server and protected-resource metadata documents; Wayground publishes no description of what it grants.
    name: full_access
  standards:
  - RFC 6749 (OAuth 2.0 authorization code)
  - RFC 7636 (PKCE)
  - RFC 7591 (dynamic client registration)
  - RFC 7009 (token revocation)
  - RFC 8414 (authorization server metadata)
  - RFC 8707 (resource indicators)
  - RFC 9728 (protected resource metadata)
  token_url: https://wayground.com/_authserver/public/public/v1/oauth/token
  type: oauth2
slug: quizizz-authentication
source_filename: quizizz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://wayground.com/.well-known/oauth-authorization-server (HTTP 200, 2026-08-26) and\n  https://wayground.com/.well-known/oauth-protected-resource (HTTP 200, 2026-08-26).\n  Derived from those documents rather than from an OpenAPI, because Wayground publishes no\n  OpenAPI or developer reference.\nsummary: >-\n  Wayground's only machine-facing authentication surface is an OAuth 2.1 authorization server\n  protecting its remote MCP endpoint. There is no API-key programme, no public developer\n  console, and no documented token issuance for a REST API - because there is no public REST\n  API. Human and LMS-facing authentication is separate and is handled through LTI 1.3 launches\n  and SSO/rostering with Clever, ClassLink and Google Classroom.\nschemes:\n- name: wayground_mcp_oauth\n  type: oauth2\n  flow: authorizationCode\n  pkce_required: true\n  pkce_methods:\n  - S256\n  authorization_url: https://wayground.com/_authserver/public/public/v1/oauth/authorize\n\
  \  token_url: https://wayground.com/_authserver/public/public/v1/oauth/token\n  revocation_url: https://wayground.com/_authserver/public/public/v1/oauth/revoke\n  registration_url: https://wayground.com/_authserver/public/public/v1/oauth/register\n  refresh_tokens: true\n  client_type: public\n  client_authentication:\n  - none\n  dynamic_client_registration: true\n  resource_indicators: true\n  scopes:\n  - name: full_access\n    description: >-\n      The single scope Wayground advertises. Verbatim from scopes_supported in both the\n      authorization-server and protected-resource metadata documents; Wayground publishes no\n      description of what it grants.\n  applies_to:\n  - https://wayground.com/_quizizzmcp/main/mcp\n  standards:\n  - RFC 6749 (OAuth 2.0 authorization code)\n  - RFC 7636 (PKCE)\n  - RFC 7591 (dynamic client registration)\n  - RFC 7009 (token revocation)\n  - RFC 8414 (authorization server metadata)\n  - RFC 8707 (resource indicators)\n  - RFC 9728 (protected resource\
  \ metadata)\nnon_api_authentication:\n- name: LTI 1.3 launch\n  type: openIdConnect\n  description: >-\n    Learning-platform users reach Wayground through an LTI launch from Canvas, Schoology,\n    Blackboard or Moodle. The LTI 1.3 handshake is an OIDC third-party-initiated login with a\n    signed id_token; Wayground generates the client ID and JSON configuration per institution\n    from https://wayground.com/lti/admin/canvas/integration rather than publishing a static\n    tool configuration.\n  docs: https://help.wayground.com/support/solutions/articles/158000403884-integrate-wayground-with-canvas-via-lti-as-an-administrator\n- name: Rostering and SSO\n  type: sso\n  description: >-\n    Clever, ClassLink and Google Classroom provide sign-in and roster sync for schools and\n    districts. Credentials are issued and managed by those platforms, not by Wayground.\n  docs: https://wayground.com/home/integrations\ngaps:\n- >-\n  No OIDC discovery document is served (/.well-known/openid-configuration\
  \ returns an S3\n  AccessDenied 403), so an OIDC client cannot auto-configure against Wayground even though the\n  OAuth AS metadata is present.\n- >-\n  full_access is the only scope. There is no read/write split, no per-resource scope, and no\n  published description of what it authorises - an agent operator cannot grant a narrow\n  permission.\n- No public documentation of the OAuth flow or of the MCP endpoint it protects.\n- No static, publicly fetchable LTI 1.3 tool configuration or JWKS URL.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quizizz/refs/heads/main/authentication/quizizz-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Education
- EdTech
- K-12
- Learning
- Assessment
- Artificial Intelligence
- MCP
- LTI
- Rostering
- Single Sign-On
---
