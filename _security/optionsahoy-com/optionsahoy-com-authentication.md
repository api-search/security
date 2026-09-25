---
anonymous_access: false
api_key_in: []
api_specs:
- filename: optionsahoy-com-openapi.json
  format: json
  label: OptionsAhoy Calculator API
  slug: optionsahoy-calculator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optionsahoy-com/refs/heads/main/openapi/optionsahoy-com-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Optionsahoy Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: OptionsAhoy declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: OptionsAhoy
provider_slug: optionsahoy-com
scheme_count: 0
schemes: []
slug: optionsahoy-com-authentication
source_filename: optionsahoy-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/optionsahoy-com-openapi.json\ndocs:\n- https://optionsahoy.com/for-agents\n- https://github.com/AlvisoOculus/optionsahoy-mcp/blob/main/SECURITY.md\n- https://github.com/AlvisoOculus/optionsahoy-mcp/blob/main/llms-install.md\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  bearer: false\n  credential_classes: 0\n  headline: >-\n    No authentication on any surface, by design and by statement. The OpenAPI 3.1.0 contract declares no\n    securitySchemes and no security requirement; the for-agents page says \"No API key, no OAuth\"; llms.txt\n    says \"no auth, no install\"; the agent card says \"OptionsAhoy's API is keyless\"; SECURITY.md says \"No\n    accounts, no authentication, no stored user data.\" The MCP server answers initialize and tools/list\n    anonymously and serves no OAuth/OIDC discovery documents (/.well-known/oauth-authorization-server,\n    /.well-known/oauth-protected-resource and /.well-known/openid-configuration\
  \ all 404). This is a genuine\n    zero-credential public API, not an undocumented gate: derive-authentication.py correctly produced no\n    profile, and this file records the absence from the provider's own statements so the auth model reads as\n    \"open\" rather than \"unknown\".\nschemes: []\nsurfaces:\n- {surface: REST, endpoint: 'https://optionsahoy.com/api/v1/*', auth: none, evidence: 'OpenAPI has no securitySchemes/security; live GET /api/v1 200 and POST /api/v1/qsbs 400 (validation, not 401) with no credential'}\n- {surface: MCP, endpoint: 'https://optionsahoy.com/mcp', auth: none, evidence: 'initialize/tools/list/resources/list/prompts/list all 200 anonymously; no RFC 9728 or RFC 8414 metadata on the host; CORS allows any origin'}\n- {surface: A2A, endpoint: 'https://optionsahoy.com/a2a', auth: none, evidence: 'agent card declares no securitySchemes/security; POST message/send with empty params returned a JSON-RPC -32602 validation error, not an auth challenge'}\n- {surface:\
  \ stdio package, install: 'npx -y optionsahoy-mcp', auth: none, evidence: 'llms-install.md: \"Requirements: Node 20 or newer. No environment variables are needed.\"'}\naccess_controls_that_exist_instead:\n- {kind: abuse rate limiting at the edge, evidence: 'privacy policy: a hash of the caller IP is stored so the server can \"rate limit abusive traffic without keeping the address itself\"; no threshold published (rate-limits/optionsahoy-com-rate-limits.yml)'}\n- {kind: license terms, evidence: 'OpenAPI info.license: \"Proprietary. Free for non-commercial use during beta.\" — a legal constraint, not a technical one'}\n- {kind: Cloudflare Turnstile, scope: 'the beta-signup and scenario-email FORMS on the website only, per the privacy policy; not the API'}\nsessions:\n  mcp: 'mcp-session-id assigned in the initialize response and echoed by the client (Streamable HTTP); a session handle, not a credential'\nmtls: false\nsigned_requests: false\nnote: >-\n  Because nothing authenticates the caller,\
  \ an agent should treat every response as public data and treat its\n  own inputs as leaving the user's device (llms.txt: \"an agent that calls them is sending inputs over the\n  network by design\"); SECURITY.md states the inputs are not retained.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optionsahoy-com/refs/heads/main/authentication/optionsahoy-com-authentication.yml
summary_line: 0 schemes
tags:
- Equity Compensation
- Tax
- Stock Options
- Financial Planning
- Personal Finance
- Fintech
- Calculators
- MCP
- A2A
- Agent-Native
- Deterministic
- United States
---
