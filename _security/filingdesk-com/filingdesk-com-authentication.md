---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Filingdesk Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: FilingDesk declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FilingDesk
provider_slug: filingdesk-com
scheme_count: 1
schemes:
- description: 'The FilingDesk Data MCP server is public and unauthenticated. The /mcp/ page states it plainly: "A free, public MCP server ... no API key, no account, no rate card" and "Streamable HTTP transport -- JSON-RPC 2.0 over POST -- no authentication". Any MCP client can connect with only the endpoint URL https://filingdesk.com/api/mcp.'
  evidence_quote: Streamable HTTP transport -- JSON-RPC 2.0 over POST -- no authentication -- 51 jurisdictions
  type: none
slug: filingdesk-com-authentication
source_filename: filingdesk-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://filingdesk.com/mcp/\ndocs: https://filingdesk.com/mcp/\nname: FilingDesk authentication\nschemes:\n- type: none\n  description: >-\n    The FilingDesk Data MCP server is public and unauthenticated. The /mcp/ page states it plainly:\n    \"A free, public MCP server ... no API key, no account, no rate card\" and \"Streamable HTTP\n    transport -- JSON-RPC 2.0 over POST -- no authentication\". Any MCP client can connect with only\n    the endpoint URL https://filingdesk.com/api/mcp.\n  evidence_quote: \"Streamable HTTP transport -- JSON-RPC 2.0 over POST -- no authentication -- 51 jurisdictions\"\nnotes:\n- >-\n  submit_order has a real-world side effect (notifies a FilingDesk specialist) but is not\n  authenticated at the transport layer. The server gates it on an in-tool consent flag\n  (userConfirmed) rather than a credential, and nothing is charged at submission -- a specialist\n  verifies the name and emails a payment\
  \ link separately.\n"
source_yaml_url: https://artifacts.apis.io/filingdesk-com/authentication/filingdesk-com-authentication.yml
summary_line: 1 scheme
tags:
- LLC Formation
- Business Formation
- Company Registration
- EIN
- Operating Agreement
- Registered Agent
- Compliance
- AI Agents
- MCP
- SMB
---
