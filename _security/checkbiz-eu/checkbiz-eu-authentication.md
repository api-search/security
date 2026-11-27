---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CheckBiz.eu Authentication
name_suffix: Authentication
oauth_flows: []
overview: CheckBiz.eu declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CheckBiz.eu
provider_slug: checkbiz-eu
scheme_count: 1
schemes:
- applies_to:
  - REST GET https://api.checkbiz.eu/v1/merchant-check
  - remote MCP server https://api.checkbiz.eu/mcp (sent as an HTTP header in the mcpServers config)
  evidence: 'curl "https://api.checkbiz.eu/v1/merchant-check?domain=coolshop.dk" -H "X-API-Key: YOUR_KEY"'
  in: header
  name: X-API-Key
  parameter: X-API-Key
  type: apiKey
slug: checkbiz-eu-authentication
source_filename: checkbiz-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://checkbiz.eu/merchant-check/\ndocs: https://checkbiz.eu/merchant-check/\nnote: No OpenAPI is published; the auth profile is read from the Merchant Check page. Keys are issued \"in one click, no sign-up\" and the free key is anonymous (\"we store no email and no name\"). The key-issuance flow was not exercised.\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  applies_to:\n  - REST GET https://api.checkbiz.eu/v1/merchant-check\n  - remote MCP server https://api.checkbiz.eu/mcp (sent as an HTTP header in the mcpServers config)\n  evidence: 'curl \"https://api.checkbiz.eu/v1/merchant-check?domain=coolshop.dk\" -H \"X-API-Key: YOUR_KEY\"'\n"
source_yaml_url: https://artifacts.apis.io/checkbiz-eu/authentication/checkbiz-eu-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Company Verification
- Business Registers
- VAT
- Brand Protection
- Fraud Prevention
- E-Commerce
- AI Agents
- MCP
- Europe
---
