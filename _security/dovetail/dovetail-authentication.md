---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Dovetail Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dovetail secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dovetail
provider_slug: dovetail
scheme_count: 2
schemes:
- detail: 'Personal API token, opaque string prefixed "api." (e.g. api.wcF...). Presented as `Authorization: Bearer <DOVETAIL_API_TOKEN>`. Tokens expire 30 days after generation and can be manually revoked; the UI displays the key only once at creation. A token grants the data and permissions of the user who created it.'
  generation: https://dovetail.com/settings/user/account
  in: header
  name: apiToken
  parameter: Authorization
  scheme: bearer
  sources:
  - https://developers.dovetail.com/docs/authorization
  token_prefix: api.
  token_ttl_days: 30
  type: apiKey
- detail: OAuth 2.1 browser-based sign-in is supported for the hosted MCP server (https://dovetail.com/api/mcp) as an alternative to Bearer API tokens. Public-API OAuth 2.0 for third-party applications is documented as coming soon.
  name: mcpOAuth
  scheme: oauth2.1
  sources:
  - https://developers.dovetail.com/docs/mcp
  - https://developers.dovetail.com/docs/oauth-2
  status: available-for-mcp-only
  type: oauth2
slug: dovetail-authentication
source_filename: dovetail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.dovetail.com/docs/authorization\ndocs: https://developers.dovetail.com/docs/authorization\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  transport: bearer\n  oauth2_flows: []\n  note: >-\n    Dovetail's Public API authenticates with personal API tokens presented as HTTP Bearer\n    credentials. OAuth 2.0 for third-party apps is documented as \"coming soon\" and not yet\n    generally available. The hosted MCP server additionally supports OAuth 2.1 browser sign-in.\nschemes:\n  - name: apiToken\n    type: apiKey\n    in: header\n    parameter: Authorization\n    scheme: bearer\n    token_prefix: \"api.\"\n    token_ttl_days: 30\n    generation: https://dovetail.com/settings/user/account\n    detail: >-\n      Personal API token, opaque string prefixed \"api.\" (e.g. api.wcF...). Presented as\n      `Authorization: Bearer <DOVETAIL_API_TOKEN>`. Tokens expire 30 days after generation\n      and can\
  \ be manually revoked; the UI displays the key only once at creation. A token\n      grants the data and permissions of the user who created it.\n    sources: [https://developers.dovetail.com/docs/authorization]\n  - name: mcpOAuth\n    type: oauth2\n    status: available-for-mcp-only\n    scheme: oauth2.1\n    detail: >-\n      OAuth 2.1 browser-based sign-in is supported for the hosted MCP server\n      (https://dovetail.com/api/mcp) as an alternative to Bearer API tokens. Public-API\n      OAuth 2.0 for third-party applications is documented as coming soon.\n    sources: [https://developers.dovetail.com/docs/mcp, https://developers.dovetail.com/docs/oauth-2]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dovetail/refs/heads/main/authentication/dovetail-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Consumer
- Customer Research
- User Research
- Customer Insights
- Customer Feedback
- Research Repository
- Analytics
- AI
- Product Management
---
