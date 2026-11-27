---
anonymous_access: false
api_key_in: []
api_specs:
- filename: founderventures-io-agents-api-openapi.yml
  format: yaml
  label: Founder Ventures Agents API
  slug: founderventures-io-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/founderventures-io/openapi/founderventures-io-agents-api-openapi.yml
- filename: founderventures-io-mcp-api-openapi.yml
  format: yaml
  label: Founder Ventures MCP API
  slug: founderventures-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/founderventures-io/openapi/founderventures-io-mcp-api-openapi.yml
auth_types: []
description: Authentication schemes as published on Founder Ventures site
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Founder Ventures Authentication
name_suffix: Authentication
oauth_flows: []
overview: Founder Ventures declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Founder Ventures
provider_slug: founderventures-io
scheme_count: 1
schemes:
- evidence: POST /api/companies/sync accepts a bearer token that is issued by hand to Founder Ventures' own pipelines.
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: founderventures-io-authentication
source_filename: founderventures-io-authentication.yml
source_heading: Authentication Profile
source_url: https://founderventures.io/auth.md
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://founderventures.io/auth.md\nsources:\n- https://founderventures.io/auth.md\n- https://founderventures.io/intel/github-copilot-usage-based-billing-token-metered-2026\n- https://founderventures.io/intel/ai-native-onboarding-replaces-product-tours-2026\ndescription: Authentication schemes as published on Founder Ventures site\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: POST /api/companies/sync accepts a bearer token that is issued by hand to Founder Ventures' own pipelines.\n  location: header\n  header: Authorization\ndocs: https://founderventures.io/auth.md\n"
source_yaml_url: https://artifacts.apis.io/founderventures-io/authentication/founderventures-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Software
- Automation
- Startups
---
