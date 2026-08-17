---
api_key_in: []
auth_types:
- delegated-user-login
description: ''
kind: authentication
layout: security
method: searched
name: Clarisights Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clarisights secures its APIs with delegated-user-login across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Clarisights
provider_slug: clarisights
scheme_count: 1
schemes:
- admin_gate:
    actor: workspace admin
    control: Settings -> Workspace -> AI access
    granularity: global on/off for the whole workspace
  authorization_detail: '"Whatever that user can see in Clarisights, the AI can see: accounts, regions, brands, reports. Nothing more." There is no parallel scope or permission tree for the agent surface — the workspace ACL is the authority.'
  authorization_model: acl-inherited
  description: The MCP client (Claude, ChatGPT, Cursor, Gemini, or any MCP-compatible tool) is pointed at a workspace-scoped connection URL and the end user signs in with their own Clarisights credentials from inside the AI client. Every call is then made on that logged-in user's behalf, using their auth, their permissions, and their history.
  enrollment:
  - action: Workspace admin enables AI access (Settings -> Workspace -> AI access).
    step: 1
  - action: Signed-in user opens their MCP settings page and copies the workspace connection URL.
    step: 2
  - action: User pastes the URL into their AI client and signs in with their Clarisights account.
    step: 3
  name: clarisights-workspace-login
  scopes: []
  scopes_note: No OAuth scope surface is published, so scopes/ is deliberately not emitted. Authorization is entirely ACL-inherited rather than scope-granted.
  sources:
  - https://clarisights.com/marketing-data-mcp
  surface: mcp
  type: delegated-user-login
slug: clarisights-authentication
source_filename: clarisights-authentication.yml
source_heading: Authentication Profile
source_url: https://clarisights.com/marketing-data-mcp
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://clarisights.com/marketing-data-mcp\nsources:\n- https://clarisights.com/marketing-data-mcp\n- https://clarisights.com/llms.txt\n- https://github.com/clarisights/claude-plugins\nnote: >-\n  Derived-from-spec was not possible: Clarisights publishes no OpenAPI, so\n  derive-authentication.py produced zero schemes (0 spec files). This profile is\n  SEARCHED from the provider's own Marketing Data MCP documentation, which\n  describes the auth model for the only programmatic surface the company ships.\nsummary:\n  types: [delegated-user-login]\n  api_key_in: []\n  oauth2_flows: []\n  api_keys_issued: false\n  api_keys_note: >-\n    Explicitly none. The docs say it twice — \"no separate tokens to manage\" and\n    \"No separate tokens, no parallel permission tree.\" There is no developer\n    key-issuance surface anywhere on the site.\nschemes:\n- name: clarisights-workspace-login\n  type: delegated-user-login\n  surface:\
  \ mcp\n  sources: [https://clarisights.com/marketing-data-mcp]\n  description: >-\n    The MCP client (Claude, ChatGPT, Cursor, Gemini, or any MCP-compatible tool)\n    is pointed at a workspace-scoped connection URL and the end user signs in\n    with their own Clarisights credentials from inside the AI client. Every call\n    is then made on that logged-in user's behalf, using their auth, their\n    permissions, and their history.\n  authorization_model: acl-inherited\n  authorization_detail: >-\n    \"Whatever that user can see in Clarisights, the AI can see: accounts,\n    regions, brands, reports. Nothing more.\" There is no parallel scope or\n    permission tree for the agent surface — the workspace ACL is the authority.\n  admin_gate:\n    control: Settings -> Workspace -> AI access\n    granularity: global on/off for the whole workspace\n    actor: workspace admin\n  enrollment:\n  - step: 1\n    action: Workspace admin enables AI access (Settings -> Workspace -> AI access).\n\
  \  - step: 2\n    action: Signed-in user opens their MCP settings page and copies the workspace connection URL.\n  - step: 3\n    action: User pastes the URL into their AI client and signs in with their Clarisights account.\n  scopes: []\n  scopes_note: >-\n    No OAuth scope surface is published, so scopes/ is deliberately not emitted.\n    Authorization is entirely ACL-inherited rather than scope-granted.\nsso:\n  supported: true\n  evidence: >-\n    The Effective Self-Service page (linked from the provider llms.txt) states\n    \"row/column-level security with SSO\". No SSO protocol, IdP list, or metadata\n    endpoint is published publicly.\n  protocols_published: false\noidc_discovery:\n  probed: true\n  result: none\n  detail: >-\n    /.well-known/openid-configuration, /.well-known/oauth-authorization-server\n    and /.well-known/oauth-protected-resource all return 404 on clarisights.com\n    and 404 on app.clarisights.com (probed 2026-08-13). See\n    well-known/clarisights-well-known.yml.\n\
  data_handling:\n  stores_user_data: false\n  evidence: >-\n    \"The MCP server is an interface, not a store. Your data stays in\n    Clarisights.\" Documented GDPR-compliant with no region-specific data\n    residency wrinkles.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarisights/refs/heads/main/authentication/clarisights-authentication.yml
summary_line: delegated-user-login · 1 scheme
tags:
- Company
- Marketing Analytics
- Marketing Intelligence
- Business Intelligence
- Data Integration
- Reporting
- Dashboards
- MCP
- AI
---
