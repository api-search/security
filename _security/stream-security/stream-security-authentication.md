---
api_key_in: []
api_specs:
- filename: stream-security-api-openapi.json
  format: json
  label: Stream Security API
  slug: stream-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stream-security/refs/heads/main/openapi/stream-security-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Stream Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stream.Security secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stream.Security
provider_slug: stream-security
scheme_count: 1
schemes:
- applies_to: all 34 operations
  bearerFormat: JWT
  header: 'Authorization: Bearer <API token>'
  lifecycle:
    automatic_revocation:
    - When a user account is deactivated, all tokens they created are revoked and labelled as such.
    - When a user is assigned a lower role, tokens exceeding the new role's permissions are revoked.
    - When a user is assigned a higher role, existing tokens remain active; new tokens reflect the updated role.
    revocation: Immediate on admin action. Revoked tokens remain visible in the management view for 90 days.
    rotation: manual - no programmatic token-issuance or rotation endpoint exists in the API
  name: BearerAuth
  provisioning:
    disclosure: The full token is displayed exactly once at creation and must be copied and stored securely.
    fields:
    - name (required)
    - description (optional)
    - permission (Read & Write / Read Only - Read Only documented as "supported soon")
    - scope (organization-wide or selected workspaces; Workspace Admins are limited to their own)
    - expiration (1 day, 7 days, 30 days, 90 days, 1 year, or never)
    location: Stream UI -> Organization Settings or Workspace Settings -> API Token Management
    who: Organization Admins (all tokens, all workspaces) and Workspace Admins (their workspace only)
  scheme: bearer
  sources:
  - openapi/stream-security-api-openapi.json
  type: http
slug: stream-security-authentication
source_filename: stream-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: openapi/stream-security-api-openapi.json\ndocs: https://docs.streamsec.io/docs/token-management\ndocs_secondary: https://docs.streamsec.io/reference/getting-started-with-stream-api\nsummary:\n  types:\n  - http\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  api_key_header: false\n  note: >-\n    A single scheme covers all 34 operations. There is no OAuth, no OIDC and no mTLS on the API.\n    SAML SSO exists but is for CONSOLE sign-in only (Okta, Azure AD/Entra, Google Workspace and AWS\n    documented as IdPs) - it does not issue API credentials.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  header: 'Authorization: Bearer <API token>'\n  applies_to: all 34 operations\n  sources:\n  - openapi/stream-security-api-openapi.json\n  provisioning:\n    location: Stream UI -> Organization Settings or Workspace Settings -> API Token Management\n    who: Organization Admins (all\
  \ tokens, all workspaces) and Workspace Admins (their workspace only)\n    fields:\n    - name (required)\n    - description (optional)\n    - permission (Read & Write / Read Only - Read Only documented as \"supported soon\")\n    - scope (organization-wide or selected workspaces; Workspace Admins are limited to their own)\n    - expiration (1 day, 7 days, 30 days, 90 days, 1 year, or never)\n    disclosure: >-\n      The full token is displayed exactly once at creation and must be copied and stored securely.\n  lifecycle:\n    rotation: manual - no programmatic token-issuance or rotation endpoint exists in the API\n    revocation: >-\n      Immediate on admin action. Revoked tokens remain visible in the management view for 90 days.\n    automatic_revocation:\n    - When a user account is deactivated, all tokens they created are revoked and labelled as such.\n    - When a user is assigned a lower role, tokens exceeding the new role's permissions are revoked.\n    - When a user is assigned\
  \ a higher role, existing tokens remain active; new tokens reflect the\n      updated role.\ntenancy:\n  header: workspace\n  required: false\n  behaviour: >-\n    Requests default to the workspace bound to the token. A token with multi-workspace access\n    targets one by sending its ID in the `workspace` header.\n  discovery: GET /workspaces\n  docs: https://docs.streamsec.io/docs/how-to-get-your-workspace-id\n  mcp_divergence: >-\n    The MCP server uses the header name `customer` for the same workspace ID, and supports only one\n    workspace per token.\nscopes:\n  model: none\n  note: >-\n    No OAuth scopes. Authorization is a two-axis model - a coarse permission level (Read & Write /\n    Read Only) crossed with a workspace scope. Consequently no scopes/ artifact is emitted:\n    derive-oauth-scopes.py found no oauth2 securityScheme, which is the correct result rather than\n    a gap in the pass.\nerrors:\n  '401': Authorization not provided - missing, malformed or expired token.\n\
  \  '403': Insufficient access - authenticated but outside the token's permission level or workspace scope.\n  see: errors/stream-security-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stream-security/refs/heads/main/authentication/stream-security-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cloud Security
- Cloud Detection and Response
- CNAPP
- Threat Detection
- Vulnerability Management
- Kubernetes
- Observability
- DevSecOps
- Artificial Intelligence
---
