---
anonymous_access: false
api_key_in: []
api_specs:
- filename: filings-tools-account-api-openapi.yml
  format: yaml
  label: filings.tools Account API
  slug: filings-tools-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filings-tools/openapi/filings-tools-account-api-openapi.yml
- filename: filings-tools-filings-api-openapi.yml
  format: yaml
  label: filings.tools Filings API
  slug: filings-tools-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filings-tools/openapi/filings-tools-filings-api-openapi.yml
auth_types: []
description: Authentication methods as described on the page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: filings.tools Authentication
name_suffix: Authentication
oauth_flows: []
overview: filings.tools declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: filings.tools
provider_slug: filings-tools
scheme_count: 1
schemes:
- evidence: FREE API KEY 200 calls a day, for your email.
  how_to_obtain: Get a free key via the form on the page.
  name: Free API Key
  type: apiKey
slug: filings-tools-authentication
source_filename: filings-tools-authentication.yml
source_heading: Authentication Profile
source_url: https://filings.tools/billing/free
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://filings.tools/billing/free\nsources:\n- https://filings.tools/billing/free\ndescription: Authentication methods as described on the page.\nschemes:\n- type: apiKey\n  name: Free API Key\n  evidence: FREE API KEY 200 calls a day, for your email.\n  how_to_obtain: Get a free key via the form on the page.\ndocs: https://filings.tools/billing/free\n"
source_yaml_url: https://artifacts.apis.io/filings-tools/authentication/filings-tools-authentication.yml
summary_line: 1 scheme
tags:
- SEC Filings
- 10-K
- 10-Q
- 8-K
- Risk Factors
- Financial Documents
- Diff
- MCP
- Developer API
---
