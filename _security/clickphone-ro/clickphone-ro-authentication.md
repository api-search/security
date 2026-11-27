---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ClickPhone Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClickPhone declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ClickPhone
provider_slug: clickphone-ro
scheme_count: 2
schemes:
- applies_to:
  - ClickPhone SMS API
  description: API-only token the user generates in the ClickPhone web account, API section; it can be regenerated or deleted at any time. Same account as the ClickPhone telephony service; no separate account needed.
  format: 'Authorization: Bearer TOKENUL_TAU'
  header: Authorization
  in: header
  name: bearerToken
  scheme: bearer
  type: http
- applies_to:
  - ClickPhone MCP Server
  description: The MCP server at https://www.clickphone.ro/mcp is documented as public and unauthenticated (per apis.yml / mcp.html).
  name: none
  type: none
slug: clickphone-ro-authentication
source_filename: clickphone-ro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.clickphone.ro/sms-api.html\ndocs: https://www.clickphone.ro/sms-api.html\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer TOKENUL_TAU'\n  description: API-only token the user generates in the ClickPhone web account, API section; it can be regenerated or deleted at any time. Same account as the ClickPhone telephony service; no separate account needed.\n  applies_to: [ClickPhone SMS API]\n- name: none\n  type: none\n  description: The MCP server at https://www.clickphone.ro/mcp is documented as public and unauthenticated (per apis.yml / mcp.html).\n  applies_to: [ClickPhone MCP Server]\nnote: No OAuth is documented, so no scopes artifact. Full API documentation is available only authenticated, inside the account.\n"
source_yaml_url: https://artifacts.apis.io/clickphone-ro/authentication/clickphone-ro-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Telecommunications
- VoIP
- Cloud PBX
- SIP Trunk
- SMS
- Call Center
- MCP
- Romania
---
