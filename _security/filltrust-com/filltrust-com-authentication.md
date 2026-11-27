---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: FillTrust Authentication
name_suffix: Authentication
oauth_flows: []
overview: FillTrust declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FillTrust
provider_slug: filltrust-com
scheme_count: 1
schemes:
- description: 'The FillTrust MCP server at https://www.filltrust.com/api/mcp is

    documented as free, read-only and anonymous -- "no account" and

    "needs no account". No API key, OAuth token or authorization header

    is required to call tools/list or any of the five tools.

    '
  docs: https://www.filltrust.com/mcp
  name: none
  type: none
slug: filltrust-com-authentication
source_filename: filltrust-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://www.filltrust.com/mcp\nschemes:\n- name: none\n  type: none\n  description: |\n    The FillTrust MCP server at https://www.filltrust.com/api/mcp is\n    documented as free, read-only and anonymous -- \"no account\" and\n    \"needs no account\". No API key, OAuth token or authorization header\n    is required to call tools/list or any of the five tools.\n  docs: https://www.filltrust.com/mcp\nnote: |\n  There is no documented REST/OpenAPI surface. The web application itself\n  uses password-based sessions with optional TOTP two-factor auth and\n  rate-limited authentication endpoints (source:\n  https://www.filltrust.com/security), but those are human-facing\n  session endpoints and the product documentation states the API\n  backend \"is not reachable from the public internet.\"\n"
source_yaml_url: https://artifacts.apis.io/filltrust-com/authentication/filltrust-com-authentication.yml
summary_line: 1 scheme
tags:
- Security Questionnaires
- Vendor Risk
- Compliance Automation
- Trust Center
- SOC 2
- CAIQ
- MCP
- AI Drafting
---
