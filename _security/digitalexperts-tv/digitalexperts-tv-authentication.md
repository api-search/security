---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Digital Experts Authentication
name_suffix: Authentication
oauth_flows: []
overview: Digital Experts declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Digital Experts
provider_slug: digitalexperts-tv
scheme_count: 1
schemes:
- applies_to:
  - https://mcp.digitalexperts.tv/mcp
  - https://digitalexperts.tv/data/hypotheses.json
  - https://digitalexperts.tv/data/benchmarks.json
  evidence: Read-only, no sign-up, up to 60 requests per minute.
  name: anonymous
  type: none
slug: digitalexperts-tv-authentication
source_filename: digitalexperts-tv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://digitalexperts.tv/en/data\ndocs: https://digitalexperts.tv/en/data\nsummary: No authentication. The MCP server is documented as \"Read-only, no sign-up, up to 60 requests per minute\", and the open dataset is static JSON served by plain GET under CC BY 4.0.\nschemes:\n- type: none\n  name: anonymous\n  applies_to:\n  - https://mcp.digitalexperts.tv/mcp\n  - https://digitalexperts.tv/data/hypotheses.json\n  - https://digitalexperts.tv/data/benchmarks.json\n  evidence: Read-only, no sign-up, up to 60 requests per minute.\n"
source_yaml_url: https://artifacts.apis.io/digitalexperts-tv/authentication/digitalexperts-tv-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Marketing
- Marketing Agency
- B2B Marketing
- Consulting
- Lead Generation
- Open Data
- AI Automation
- MCP
---
