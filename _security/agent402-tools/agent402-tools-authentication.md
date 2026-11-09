---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agent402-tools-api-openapi.json
  format: json
  label: 'Agent402: 500+ pay-per-call tools for AI agents over x402 + MPP Api API'
  slug: agent402-500-pay-per-call-tools-for-ai-agents-over-x402-mpp-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent402-tools/openapi/_original/agent402-tools-api-openapi.json
auth_types: []
description: Authentication schemes for Agent402 Tools
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agent402 Tools Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent402 Tools declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Agent402 Tools
provider_slug: agent402-tools
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer a402_…'
  header: Authorization
  how_to_obtain: Purchased via card at /reports or obtained from /credits endpoint
  location: header
  name: prepaid credits key
  type: http-bearer
slug: agent402-tools-authentication
source_filename: agent402-tools-authentication.yml
source_heading: Authentication Profile
source_url: https://agent402.tools/docs/Getting-Started
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agent402.tools/docs/Getting-Started\nsources:\n- https://agent402.tools/docs/Getting-Started\ndescription: Authentication schemes for Agent402 Tools\nschemes:\n- type: http-bearer\n  name: prepaid credits key\n  evidence: 'Authorization: Bearer a402_…'\n  location: header\n  header: Authorization\n  how_to_obtain: Purchased via card at /reports or obtained from /credits endpoint\nnote: No other authentication schemes (apiKey, oauth2, http-basic, jwt, hmac, mtls, other) are documented on the page.\ndocs: https://agent402.tools/docs/Getting-Started\n"
source_yaml_url: https://artifacts.apis.io/agent402-tools/authentication/agent402-tools-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Marketplace
- Tools
- Pay-per-call
- Integration
---
