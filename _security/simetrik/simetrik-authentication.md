---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Simetrik Authentication
name_suffix: Authentication
oauth_flows: []
overview: Simetrik declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Simetrik
provider_slug: simetrik
scheme_count: 0
schemes: []
slug: simetrik-authentication
source_filename: simetrik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: >-\n  Live anonymous fetch of https://mcp.us.simetrik.com/.well-known/oauth-authorization-server and\n  https://mcp.us.simetrik.com/.well-known/oauth-protected-resource/mcp (both HTTP 200), the 401\n  WWW-Authenticate challenge from https://mcp.us.simetrik.com/mcp, plus\n  https://docs.simetrik.com/mcp/connect, https://docs.simetrik.com/cli/reference/account/login and\n  https://docs.simetrik.com/administration, 2026-08-27.\nnote: >-\n  Derived from OpenAPI securitySchemes was not possible - Simetrik publishes no OpenAPI. This profile\n  is built from the provider's live OAuth metadata documents and its own auth documentation instead,\n  which is a stronger source than a spec declaration because the metadata is served by the running\n  authorization server.\nsurfaces:\n- surface: MCP server\n  endpoint: https://mcp.us.simetrik.com/mcp\n  scheme_type: oauth2\n  spec: MCP authorization - OAuth 2.1 with RFC 9728 protected resource\
  \ metadata\n  flows:\n  - flow: authorizationCode\n    authorization_url: https://mcp.us.simetrik.com/authorize\n    token_url: https://mcp.us.simetrik.com/token\n    refresh_url: https://mcp.us.simetrik.com/token\n    pkce: S256\n    pkce_required: true\n    scopes:\n      openid: OpenID Connect authentication of the Simetrik user\n      profile: Basic profile claims for the signed-in Simetrik user\n      email: Email address of the signed-in Simetrik user\n  dynamic_client_registration:\n    supported: true\n    registration_endpoint: https://mcp.us.simetrik.com/register\n    client_id_metadata_document_supported: true\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic, private_key_jwt, none]\n  grant_types: [authorization_code, refresh_token]\n  response_types: [code]\n  bearer_methods: [header]\n  challenge:\n    http_status: 401\n    www_authenticate: >-\n      Bearer resource_metadata=\"https://mcp.us.simetrik.com/.well-known/oauth-protected-resource/mcp\"\n\
  \  api_key: false\n  api_key_note: >-\n    Documented explicitly: \"There's no API key to create, copy or rotate - your client never handles a\n    Simetrik credential.\" Removing the server from the client ends access; there is no key left to\n    revoke.\n- surface: CLI\n  endpoint: BFF, selected by an --env preset; not a published host\n  scheme_type: oauth2\n  command: simetrik login\n  flows:\n  - flow: authorizationCode\n    provider: Auth0\n    browser: true\n    note: >-\n      Default browser-based login. --no-browser prints the URL instead of opening it.\n  - flow: deviceCode\n    provider: Auth0\n    note: >-\n      `simetrik login --device` uses the device authorization flow with no browser, documented for\n      SSH, CI and agents.\n  token_storage: >-\n    The resulting BFF token is written to a named profile in ~/.simetrik/config.json. `simetrik config`\n    shows it masked (last 8 characters only). `simetrik logout` revokes it server-side and clears it\n    locally.\n \
  \ ttl_controls:\n  - flag: --ttl\n    unit: hours\n    controls: CLI session lifetime\n  - flag: --access-token-ttl\n    unit: seconds\n    controls: Access token lifetime\n  custom_deployments:\n    flag: --url\n    note: >-\n      A raw BFF base URL plus an optional bearer --token may be set on a profile, documented as\n      reserved for custom or self-hosted deployments. Passing both --env and --url is rejected.\nauthorization_model:\n  type: rbac\n  description: >-\n    Access is the signed-in user's own Simetrik permissions - the MCP server \"acts as you. A Viewer\n    sees what a Viewer sees.\" Two independent gates control programmatic access at all: the workspace\n    must be enabled for CLI/agent access, and the user's role must carry the \"Use CLI\" permission.\n    The same tool can succeed in one workspace and fail in another for the same account.\n  administration: Roles, permissions and users are managed in app.simetrik.com, not via CLI or MCP.\n  enterprise_identity:\n\
  \    sso: true\n    provider: Microsoft Entra ID (Azure Active Directory)\n    mechanism: >-\n      Simetrik roles are provisioned to users through Entra ID security groups, so access and role\n      assignment come from the corporate directory rather than being set by hand in the platform.\n    docs: https://docs.simetrik.com/administration\naudit: Every MCP call is documented as authenticated, authorized and logged.\ndocs:\n  mcp_connect: https://docs.simetrik.com/mcp/connect\n  cli_login: https://docs.simetrik.com/cli/getting-started/login\n  enable_cli_role: https://docs.simetrik.com/cli/getting-started/login/enable-cli-role\n  administration: https://docs.simetrik.com/administration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simetrik/refs/heads/main/authentication/simetrik-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Reconciliation
- Financial Operations
- Payments
- Accounting
- FinTech
- Financial Close
- Data Integration
- Agents
- MCP
- Latin America
---
