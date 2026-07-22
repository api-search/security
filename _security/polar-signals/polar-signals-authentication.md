---
api_key_in: []
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Polar Signals Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Polar Signals secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Polar Signals
provider_slug: polar-signals
scheme_count: 3
schemes:
- applies_to: Polar Signals Cloud gRPC/Connect API and profiling data plane
  header: Authorization
  in: header
  name: ServiceAccountToken
  notes: 'Service-account tokens replace the older JWT approach and provide granular per-token permissions via RBAC roles. Passed as Authorization: Bearer; the agent uses --remote-store-bearer-token-file. The target project is selected separately through the projectID gRPC metadata header (--remote-store-grpc-headers), decoupling project assignment from token permissions. Tokens are shown once at creation; only a hash is stored.'
  scheme: bearer
  token_format: psc_v1_<64-hex>
  type: http
- authorization_endpoint: https://cloud.polarsignals.com/login/cli
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://identity.polarsignals.com
  name: OAuth2 (CLI / dashboard login)
  pkce: S256
  registration_endpoint: https://api.polarsignals.com/api/oauth/register
  scopes:
  - openid
  - email
  - groups
  - profile
  - offline_access
  source: well-known/polar-signals-oauth-authorization-server.json
  token_endpoint: https://identity.polarsignals.com/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
- name: SSO / OIDC
  notes: Organizations can enable Single Sign-On (SAML/OIDC) with a default role for SSO-provisioned users. Configured via OrganizationService EnableSSO / GetSSOSettings / UpdateSSODefaultRole.
  provider: Dex-based OIDC (github.com/polarsignals/dex)
  type: openIdConnect
slug: polar-signals-authentication
source_filename: polar-signals-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource:\n- https://www.polarsignals.com/docs/generating-tokens\n- https://www.polarsignals.com/docs/single-sign-on\n- well-known/polar-signals-oauth-authorization-server.json\nsummary:\n  types: [http, oauth2, openIdConnect]\n  http_scheme: bearer\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\nschemes:\n- name: ServiceAccountToken\n  type: http\n  scheme: bearer\n  token_format: psc_v1_<64-hex>\n  in: header\n  header: Authorization\n  applies_to: Polar Signals Cloud gRPC/Connect API and profiling data plane\n  notes: >-\n    Service-account tokens replace the older JWT approach and provide granular\n    per-token permissions via RBAC roles. Passed as Authorization: Bearer; the\n    agent uses --remote-store-bearer-token-file. The target project is selected\n    separately through the projectID gRPC metadata header\n    (--remote-store-grpc-headers), decoupling project assignment from token\n    permissions. Tokens are shown\
  \ once at creation; only a hash is stored.\n- name: OAuth2 (CLI / dashboard login)\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  issuer: https://identity.polarsignals.com\n  authorization_endpoint: https://cloud.polarsignals.com/login/cli\n  token_endpoint: https://identity.polarsignals.com/token\n  registration_endpoint: https://api.polarsignals.com/api/oauth/register\n  token_endpoint_auth_methods: [none]\n  grant_types: [authorization_code, refresh_token]\n  scopes: [openid, email, groups, profile, offline_access]\n  source: well-known/polar-signals-oauth-authorization-server.json\n- name: SSO / OIDC\n  type: openIdConnect\n  provider: Dex-based OIDC (github.com/polarsignals/dex)\n  notes: >-\n    Organizations can enable Single Sign-On (SAML/OIDC) with a default role for\n    SSO-provisioned users. Configured via OrganizationService EnableSSO /\n    GetSSOSettings / UpdateSSODefaultRole.\nauthorization_model: >-\n  RBAC — roles, role bindings and permissions are managed\
  \ via RoleService\n  (ListRoles/CreateRole/CreateRoleBinding/ListPermissions) and enforced by\n  AuthorizationService.CanI.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polar-signals/refs/heads/main/authentication/polar-signals-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- Company
- Enterprise
- Observability
- Continuous Profiling
- Performance
- eBPF
- gRPC
- Developer Tools
- MCP
- GPU
---
