---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: DemiSignal Authentication
name_suffix: Authentication
oauth_flows: []
overview: DemiSignal declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DemiSignal
provider_slug: demisignal-com
scheme_count: 2
schemes:
- evidence_401: examples/demisignal-com-check-unauthenticated-401.json
  example: 'curl -H "Authorization: Bearer dsk_…" "https://demisignal.com/api/v1/check?domain=example.com"'
  header: Authorization
  in: header
  issuance: Create a free API key (sign in or create an account first); a key can be revoked at any time.
  key_prefix: dsk_
  name: apiKeyBearer
  required: GET /api/v1/check requires it; optional for the MCP server at https://demisignal.com/mcp
  scheme: bearer
  type: http
- description: The MCP server works with no account and no API key, sharing one daily allowance of new checks.
  name: none
  type: none
slug: demisignal-com-authentication
source_filename: demisignal-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://demisignal.com/tools/mcp-server\ndocs: https://demisignal.com/tools/mcp-server#api-keys\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  key_prefix: dsk_\n  required: GET /api/v1/check requires it; optional for the MCP server at https://demisignal.com/mcp\n  example: 'curl -H \"Authorization: Bearer dsk_…\" \"https://demisignal.com/api/v1/check?domain=example.com\"'\n  issuance: Create a free API key (sign in or create an account first); a key can be revoked at any time.\n  evidence_401: examples/demisignal-com-check-unauthenticated-401.json\n- name: none\n  type: none\n  description: The MCP server works with no account and no API key, sharing one daily allowance of new checks.\n"
source_yaml_url: https://artifacts.apis.io/demisignal-com/authentication/demisignal-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Email Authentication
- DMARC
- SPF
- DKIM
- Email Security
- DNS
- Domain Monitoring
- MCP
---
