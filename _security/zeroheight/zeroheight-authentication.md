---
api_key_in: []
api_specs:
- filename: zeroheight-open-api-v2.yml
  format: yaml
  label: Zeroheight API
  slug: zeroheight
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeroheight/refs/heads/main/openapi/zeroheight-open-api-v2.yml
auth_types: []
description: zeroheight authenticates the REST API with a paired Client ID and Access Token sent as two custom headers. There is no OAuth on the REST surface. OAuth exists only on the MCP surface, where the remote server runs a browser login flow against the customer's zeroheight team (password or SSO).
kind: authentication
layout: security
method: searched
name: Zeroheight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zeroheight declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Zeroheight
provider_slug: zeroheight
scheme_count: 4
schemes:
- description: The Client ID. May be shared; remains visible in organization/workspace settings.
  id: apiClient
  in: header
  key_prefix: zhci_
  name: X-API-CLIENT
  required: true
  type: apiKey
- description: The Access Token. Shown exactly once on creation and never again; treat like a password.
  id: apiKey
  in: header
  key_prefix: zhat_
  name: X-API-KEY
  required: true
  type: apiKey
- description: The remote MCP server at https://mcp.zeroheight.com/mcp and the local stdio server both start a browser OAuth flow. Admins/editors may sign in with username/password or SSO; viewers must use SSO. The user enters their zeroheight team subdomain, signs in, then approves the connection.
  discovery: NOT discoverable. Neither /.well-known/oauth-authorization-server (RFC 8414) nor /.well-known/oauth-protected-resource (RFC 9728) is served on mcp.zeroheight.com — both 404.
  flow: authorization_code (browser)
  id: mcpOAuth
  surface: MCP
  token_storage: ~/.zeroheight/mcp-oauth.json (local stdio server)
  type: oauth2
- description: '"MCP via link" issues each viewer a unique MCP URL that carries its own credential. The URL is the secret; zeroheight tells customers not to share their own URL. Private pages are not reachable through it.'
  id: mcpLinkCredential
  surface: MCP
  type: bearer-in-url
slug: zeroheight-authentication
source_filename: zeroheight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Zeroheight\nproviderId: zeroheight\ngenerated: '2026-08-28'\nmethod: searched\nsource: >-\n  https://help.zeroheight.com/hc/en-us/articles/35887043412251-Zeroheight-API-Authentication-token-creation ;\n  https://help.zeroheight.com/hc/en-us/articles/35887050539035 ;\n  postman/zeroheight-api.postman_collection.json ;\n  https://www.npmjs.com/package/@zeroheight/mcp-server ;\n  live 401 probes of https://zeroheight.com/open_api/v2 on 2026-08-28\ndocs: https://developers.zeroheight.com/75fe5b2ed/p/6599ef-creation\ndescription: >-\n  zeroheight authenticates the REST API with a paired Client ID and Access Token sent as two custom\n  headers. There is no OAuth on the REST surface. OAuth exists only on the MCP surface, where the\n  remote server runs a browser login flow against the customer's zeroheight team (password or SSO).\nschemes:\n  - id: apiClient\n    type: apiKey\n    in: header\n    name:\
  \ X-API-CLIENT\n    required: true\n    description: The Client ID. May be shared; remains visible in organization/workspace settings.\n    key_prefix: zhci_\n  - id: apiKey\n    type: apiKey\n    in: header\n    name: X-API-KEY\n    required: true\n    description: The Access Token. Shown exactly once on creation and never again; treat like a password.\n    key_prefix: zhat_\n  - id: mcpOAuth\n    type: oauth2\n    surface: MCP\n    flow: authorization_code (browser)\n    description: >-\n      The remote MCP server at https://mcp.zeroheight.com/mcp and the local stdio server both start a\n      browser OAuth flow. Admins/editors may sign in with username/password or SSO; viewers must use\n      SSO. The user enters their zeroheight team subdomain, signs in, then approves the connection.\n    token_storage: '~/.zeroheight/mcp-oauth.json (local stdio server)'\n    discovery: >-\n      NOT discoverable. Neither /.well-known/oauth-authorization-server (RFC 8414) nor\n      /.well-known/oauth-protected-resource\
  \ (RFC 9728) is served on mcp.zeroheight.com — both 404.\n  - id: mcpLinkCredential\n    type: bearer-in-url\n    surface: MCP\n    description: >-\n      \"MCP via link\" issues each viewer a unique MCP URL that carries its own credential. The URL is\n      the secret; zeroheight tells customers not to share their own URL. Private pages are not\n      reachable through it.\ntoken_management:\n  created_at: Developers section of organization or workspace settings\n  ownership: Tokens belong to the team, not an individual, so activity can be monitored centrally.\n  who_can_create: any member with editor permissions\n  acting_as: actions taken with a token are performed on behalf of the member who created it\n  quantity: unlimited — create and revoke as many as needed\n  rotation: tokens can be regenerated; a suspected leak should be revoked immediately\n  visibility: Access Token displayed once at creation; Client ID remains retrievable\n  use_cases:\n    - name: Measure Adoption\n    \
  \  description: Pre-defined scope set for authenticating @zeroheight/adoption-cli — package versions, component usage.\n    - name: Zapier\n      description: Pre-defined scope set for Zapier automation workflows. Requires \"Read and write\" access level for actions that change content.\n    - name: Style Dictionary Exports\n      description: Pre-defined scope set for accessing private design-token export URLs.\n  granular_scopes:\n    available: true\n    plans: Enterprise only\n    description: Granular CLI scopes for precise control over access levels beyond the pre-defined use cases.\n  access_levels:\n    - Read\n    - Read and write\nenvironment_variables:\n  - name: ZEROHEIGHT_CLIENT_ID\n    used_by: ['@zeroheight/mcp-server', '@zeroheight/adoption-cli']\n    maps_to: X-API-CLIENT\n  - name: ZEROHEIGHT_ACCESS_TOKEN\n    used_by: ['@zeroheight/mcp-server', '@zeroheight/adoption-cli']\n    maps_to: X-API-KEY\nfailure_semantics:\n  status: 401\n  body: '{\"status\":\"fail\",\"message\"\
  :\"Unauthorized\",\"data\":{\"request_id\":\"...\"}}'\n  triggers: [missing key, malformed key, invalid key]\n  observed: '2026-08-28 on GET https://zeroheight.com/open_api/v2/styleguides'\nplan_gating:\n  rest_api: Enterprise plan only — API access is not listed on Free or Starter.\n  mcp: all plans, capped at 500 calls/month on Free and Starter.\nsso:\n  supported: true\n  note: SAML/SSO sign-in for styleguide viewers; separate SSO configurations can be applied per workspace, and SSO viewer groups control which styleguides a viewer reaches over MCP.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeroheight/refs/heads/main/authentication/zeroheight-authentication.yml
summary_line: 4 schemes
tags:
- Design Systems
- Design Tokens
- Documentation
- Model Context Protocol
- Agent Readiness
- Developer Tools
- Design
- Figma
- Storybook
- Design Operations
---
