---
api_key_in: []
api_specs:
- filename: hiver-conversations-api-openapi.yml
  format: yaml
  label: Hiver Conversations API
  slug: hiver-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiver/refs/heads/main/openapi/hiver-conversations-api-openapi.yml
- filename: hiver-inbox-api-openapi.yml
  format: yaml
  label: Hiver Inbox API
  slug: hiver-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiver/refs/heads/main/openapi/hiver-inbox-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Hiver Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hiver declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hiver
provider_slug: hiver
scheme_count: 1
schemes:
- description: Account API key created by a Hiver admin under Admin Panel -> Integrations -> Developer APIs -> Create an API key. The key must be toggled on before it will authenticate. Presented verbatim as an HTTP Bearer token.
  example_request: 'curl ''https://api2.hiverhq.com/v1/inboxes'' --header ''Authorization: Bearer <your-access-token>'''
  format: Bearer <api-key>
  header: Authorization
  id: bearer_api_key
  in: header
  scheme: bearer
  source: https://developer.hiverhq.com/hiver-api
  type: http
slug: hiver-authentication
source_filename: hiver-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://developer.hiverhq.com/hiver-api\ndocs: https://help.hiverhq.com/hiver-api/hiver-api\nname: Hiver API authentication\nsummary: >-\n  The Hiver REST API authenticates with a single account-scoped API key presented as an\n  HTTP Bearer token. There is no OAuth flow, no scopes, and no per-user delegation: the key\n  is minted by a Hiver administrator in the admin panel and carries admin privileges.\nschemes:\n  - id: bearer_api_key\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer <api-key>'\n    description: >-\n      Account API key created by a Hiver admin under Admin Panel -> Integrations ->\n      Developer APIs -> Create an API key. The key must be toggled on before it will\n      authenticate. Presented verbatim as an HTTP Bearer token.\n    example_request: \"curl 'https://api2.hiverhq.com/v1/inboxes' --header 'Authorization: Bearer <your-access-token>'\"\n    source:\
  \ https://developer.hiverhq.com/hiver-api\nkey_management:\n  who_can_create: Hiver administrators only\n  location: Hiver Admin Panel -> Integrations -> Developer APIs\n  enable_toggle: true\n  privilege_model: >-\n    \"The API key will have the access privileges of an admin user.\" Hiver does not offer a\n    least-privilege or per-inbox key; every key is effectively an admin credential.\n  rotation: >-\n    Hiver documents deletion, not rotation - \"If you suspect that any of your API keys have\n    been compromised, you must take immediate action and delete them from the Hiver admin panel.\"\n  expiry: not documented\noauth:\n  api_oauth: false\n  note: >-\n    The Hiver REST API does not offer OAuth. A separate, unrelated OAuth authorization-server\n    document is served at https://hiverhq.com/.well-known/oauth-authorization-server for a\n    WordPress MCP plugin on the marketing site (scope \"mcp\"); it does not govern api2.hiverhq.com.\n    See well-known/hiver-well-known.yml\
  \ and mcp/hiver-mcp.yml.\nspec_gap:\n  observed: >-\n    openapi/hiver-api-openapi.json declares NO components.securitySchemes and NO security[].\n    Authentication is modelled as a required `Authorization` header PARAMETER on every one of\n    the 12 operations, with example \"Bearer {token}\".\n  impact: >-\n    Generated clients and agents cannot discover the auth model from the contract alone; it has\n    to be read out of the prose introduction. Adding a `bearerAuth` http/bearer securityScheme\n    and a root-level `security` block would fix it without changing a single runtime behaviour.\n  captured_in: overlays/hiver-api-overlay.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hiver/refs/heads/main/authentication/hiver-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Customer Service
- Help Desk
- Shared Inbox
- Email
- Ticketing
- Customer Support
- Collaboration
- Gmail
- Google Workspace
- Omnichannel
- Live Chat
- SaaS
- Artificial Intelligence
---
