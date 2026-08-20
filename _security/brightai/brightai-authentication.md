---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: probed
name: Brightai Authentication
name_suffix: Authentication
oauth_flows: []
overview: BrightAI secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BrightAI
provider_slug: brightai
scheme_count: 1
schemes:
- applies_to:
  - https://public.stateful.world/mcp
  - https://public.stateful.world/api/public/industries
  - https://public.stateful.world/api/public/company-teaser
  evidence: MCP initialize, tools/list, prompts/list and resources/list all returned 200 with no Authorization header. Both /api/public endpoints returned 200 unauthenticated.
  name: public-no-auth
  provider_statement: 'BrightAI''s llms.txt states "MCP server (no login): https://public.stateful.world/mcp"; the server answers /.well-known/oauth-protected-resource with {"error":"not_found","note":"This MCP server is public and requires no authentication"}.'
  type: none
slug: brightai-authentication
source_filename: brightai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live probes of https://public.stateful.world/mcp and https://public.stateful.world/api/public/*\ndocs: https://public.stateful.world/llms.txt\nnote: 'Derived by probe, not from an OpenAPI — BrightAI publishes no OpenAPI and therefore\n  no securitySchemes. The auth posture below is what the surfaces actually did when\n  called with no credentials at all.'\nsummary:\n  types:\n  - none\n  api_key_in: []\n  oauth2_flows: []\n  public_surfaces: 3\n  authenticated_surfaces: 0\n  verdict: Every published BrightAI API surface is deliberately anonymous. There is\n    no signup, no key issuance, no OAuth and no token of any kind on the public surface.\nschemes:\n- name: public-no-auth\n  type: none\n  applies_to:\n  - https://public.stateful.world/mcp\n  - https://public.stateful.world/api/public/industries\n  - https://public.stateful.world/api/public/company-teaser\n  evidence: 'MCP initialize, tools/list, prompts/list and resources/list\
  \ all returned\n    200 with no Authorization header. Both /api/public endpoints returned 200 unauthenticated.'\n  provider_statement: 'BrightAI''s llms.txt states \"MCP server (no login): https://public.stateful.world/mcp\";\n    the server answers /.well-known/oauth-protected-resource with {\"error\":\"not_found\",\"note\":\"This\n    MCP server is public and requires no authentication\"}.'\ngated_surfaces:\n- surface: Company-specific assessment (modeled dollar figures and grades for a named\n    operator)\n  gate: work-email verification of an employee of that company\n  status: 'BrightAI states this is \"rolling out shortly\" — not live at probe time.'\n  source: https://public.stateful.world/start.md\n- surface: https://api.bright.ai\n  gate: unknown — an AWS ALB that answers 403 \"Invalid Host\" at the root for an unrecognized\n    Host header and 404 for unmatched paths. Presumed the customer platform API; no\n    public documentation, no discovery document, no advertised auth\
  \ model.\n  http_status: 403\noauth_discovery:\n- url: https://public.stateful.world/.well-known/oauth-authorization-server\n  http_status: 404\n- url: https://public.stateful.world/.well-known/oauth-protected-resource\n  http_status: 404\n- url: https://www.bright.ai/.well-known/openid-configuration\n  http_status: 404\nx-evidence:\n  fetched: '2026-08-08'\n  probes:\n  - url: https://public.stateful.world/mcp\n    method: POST initialize (no Authorization header)\n    http_status: 200\n  - url: https://public.stateful.world/api/public/industries\n    http_status: 200\n  - url: https://api.bright.ai/\n    http_status: 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightai/refs/heads/main/authentication/brightai-authentication.yml
summary_line: none · 1 scheme
tags:
- Company
- Physical AI
- Industrial IoT
- Infrastructure Monitoring
- Predictive Maintenance
- Edge AI
- Foundation Models
- MCP
- Energy and Utilities
- Water and Wastewater
---
