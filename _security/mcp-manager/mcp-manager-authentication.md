---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Mcp Manager Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MCP Manager secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MCP Manager
provider_slug: mcp-manager
scheme_count: 2
schemes:
- configurable_ttl_days: 1-90 (0 = never expire)
  default_ttl_days: 90
  format: mcpm_pat_ followed by 64 hex chars (32 random bytes)
  header: Authorization
  idempotent_creation: true
  name: PersonalAccessToken
  prefix: mcpm_pat_
  scheme: bearer
  scope: acts as the creating user (carries user, role, capabilities)
  source: https://docs.mcpmanager.ai/admin-api/authentication
  storage_at_rest: SHA-256 hash only; secret shown once at creation, unrecoverable
  type: http
- audience_binding: RFC 8707 — access token aud claim must include ${ROOT_URL}/mcpm-admin/mcp
  flows:
  - flow: authorizationCode
    notes: Admin MCP server is an OAuth 2.1 protected resource. A credential-less client receives 401 with a WWW-Authenticate header advertising the protected-resource metadata document (RFC 9728); the client then runs the authorization flow.
  name: OAuth2.1
  source: https://docs.mcpmanager.ai/admin-api/authentication
  subject: token sub claim carries the resolved MCP Manager identity
  type: oauth2
slug: mcp-manager-authentication
source_filename: mcp-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.mcpmanager.ai/admin-api/authentication.md\ndocs: https://docs.mcpmanager.ai/admin-api/authentication\nsummary:\n  types: [http, oauth2]\n  bearer_formats: [personal-access-token, oauth2-jwt]\n  oauth2_flows: [authorizationCode]\n  authorization_model: capability-gating (RBAC) + workspace entitlement (ff-mcpm-admin)\nschemes:\n  - name: PersonalAccessToken\n    type: http\n    scheme: bearer\n    header: Authorization\n    prefix: mcpm_pat_\n    format: mcpm_pat_ followed by 64 hex chars (32 random bytes)\n    storage_at_rest: SHA-256 hash only; secret shown once at creation, unrecoverable\n    default_ttl_days: 90\n    configurable_ttl_days: 1-90 (0 = never expire)\n    scope: acts as the creating user (carries user, role, capabilities)\n    idempotent_creation: true  # create_access_token is idempotent by label\n    source: https://docs.mcpmanager.ai/admin-api/authentication\n  - name: OAuth2.1\n    type: oauth2\n\
  \    flows:\n      - flow: authorizationCode\n        notes: >-\n          Admin MCP server is an OAuth 2.1 protected resource. A credential-less\n          client receives 401 with a WWW-Authenticate header advertising the\n          protected-resource metadata document (RFC 9728); the client then runs\n          the authorization flow.\n    audience_binding: RFC 8707 — access token aud claim must include ${ROOT_URL}/mcpm-admin/mcp\n    subject: token sub claim carries the resolved MCP Manager identity\n    source: https://docs.mcpmanager.ai/admin-api/authentication\nauthorization:\n  entitlement: ff-mcpm-admin (plan-level; checked before authn/capability; 403 if missing, 503 if check fails)\n  capability_gating: every operation enforces the same capability as the equivalent app action\n  no_capability_ops: [whoami, list_capabilities, create_access_token, list_access_tokens, revoke_access_token]\n  capabilities_reference: https://docs.mcpmanager.ai/deployment/rbac-and-roles/capabilities\n\
  enterprise_sso:\n  protocol: OpenID Connect (OIDC) federated through Auth0\n  provisioning: SCIM 2.0 (RFC 7643 / RFC 7644)\n  source: https://docs.mcpmanager.ai/enterprise/sso.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcp-manager/refs/heads/main/authentication/mcp-manager-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- MCP
- Model Context Protocol
- AI Governance
- API Gateway
- Security
- Observability
- DLP
- Identity
- RBAC
- Enterprise
---
