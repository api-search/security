---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Payloadpier Authentication
name_suffix: Authentication
oauth_flows: []
overview: PayloadPier declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: PayloadPier
provider_slug: payloadpier
scheme_count: 1
schemes:
- evidence: Send supplier snapshots to POST /api/v1/compare using a scoped API key.
  header: PAYLOADPIER_API_KEY
  how_to_obtain: Create a scoped key in the account dashboard.
  location: header
  name: PAYLOADPIER_API_KEY
  type: apiKey
slug: payloadpier-authentication
source_filename: payloadpier-authentication.yml
source_heading: Authentication Profile
source_url: https://payloadpier.com/docs/agents
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://payloadpier.com/docs/agents\nsources:\n- https://payloadpier.com/docs/agents\nschemes:\n- type: apiKey\n  name: PAYLOADPIER_API_KEY\n  evidence: Send supplier snapshots to POST /api/v1/compare using a scoped API key.\n  location: header\n  header: PAYLOADPIER_API_KEY\n  how_to_obtain: Create a scoped key in the account dashboard.\ndocs: https://payloadpier.com/docs/agents\n"
source_yaml_url: https://artifacts.apis.io/payloadpier/authentication/payloadpier-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Pricing
- SupplierComparison
- Data Processing
---
