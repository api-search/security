---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for GTM Otto MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: GTM Otto Authentication
name_suffix: Authentication
oauth_flows: []
overview: GTM Otto declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: GTM Otto
provider_slug: gtmotto-com
scheme_count: 2
schemes:
- evidence: 'Scripts and n8n can use an API key instead: Authorization: Bearer gtm_sk… .'
  header: Authorization
  how_to_obtain: API keys are minted in the cockpit's settings.
  location: header
  name: Bearer token
  type: http-bearer
- authorize_url: https://app.gtmotto.com/connect
  evidence: You sign in once in a popup (OAuth) and the client retries the call.
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Sign in via the popup that appears on the first protected call.
  location: header
  name: OAuth
  type: oauth2
slug: gtmotto-com-authentication
source_filename: gtmotto-com-authentication.yml
source_heading: Authentication Profile
source_url: https://gtmotto.com/docs/mcp/
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gtmotto.com/docs/mcp/\nsources:\n- https://gtmotto.com/docs/mcp/\ndescription: Authentication methods for GTM Otto MCP\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Scripts and n8n can use an API key instead: Authorization: Bearer gtm_sk… .'\n  location: header\n  header: Authorization\n  how_to_obtain: API keys are minted in the cockpit's settings.\n- type: oauth2\n  name: OAuth\n  evidence: You sign in once in a popup (OAuth) and the client retries the call.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://app.gtmotto.com/connect\n  how_to_obtain: Sign in via the popup that appears on the first protected call.\ndocs: https://gtmotto.com/docs/mcp/\n"
source_yaml_url: https://artifacts.apis.io/gtmotto-com/authentication/gtmotto-com-authentication.yml
summary_line: 2 schemes
tags:
- LinkedIn Automation
- Software-as-a-Service
- Sales
- Artificial Intelligence
- Prospecting
---
