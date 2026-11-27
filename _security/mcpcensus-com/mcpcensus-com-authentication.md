---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mcpcensus-com-audit-api-openapi.yml
  format: yaml
  label: MCP Census Audit API
  slug: mcpcensus-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpcensus-com/openapi/mcpcensus-com-audit-api-openapi.yml
- filename: mcpcensus-com-changes-api-openapi.yml
  format: yaml
  label: MCP Census Changes API
  slug: mcpcensus-com-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpcensus-com/openapi/mcpcensus-com-changes-api-openapi.yml
- filename: mcpcensus-com-coverage-api-openapi.yml
  format: yaml
  label: MCP Census Coverage API
  slug: mcpcensus-com-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpcensus-com/openapi/mcpcensus-com-coverage-api-openapi.yml
- filename: mcpcensus-com-evaluations-api-openapi.yml
  format: yaml
  label: MCP Census Evaluations API
  slug: mcpcensus-com-evaluations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpcensus-com/openapi/mcpcensus-com-evaluations-api-openapi.yml
- filename: mcpcensus-com-policies-api-openapi.yml
  format: yaml
  label: MCP Census Policies API
  slug: mcpcensus-com-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpcensus-com/openapi/mcpcensus-com-policies-api-openapi.yml
- filename: mcpcensus-com-preflight-api-openapi.yml
  format: yaml
  label: MCP Census Preflight API
  slug: mcpcensus-com-preflight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpcensus-com/openapi/mcpcensus-com-preflight-api-openapi.yml
- filename: mcpcensus-com-recent-api-openapi.yml
  format: yaml
  label: MCP Census Recent API
  slug: mcpcensus-com-recent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpcensus-com/openapi/mcpcensus-com-recent-api-openapi.yml
- filename: mcpcensus-com-resolve-api-openapi.yml
  format: yaml
  label: MCP Census Resolve API
  slug: mcpcensus-com-resolve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpcensus-com/openapi/mcpcensus-com-resolve-api-openapi.yml
- filename: mcpcensus-com-search-api-openapi.yml
  format: yaml
  label: MCP Census Search API
  slug: mcpcensus-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpcensus-com/openapi/mcpcensus-com-search-api-openapi.yml
- filename: mcpcensus-com-server-api-openapi.yml
  format: yaml
  label: MCP Census Server API
  slug: mcpcensus-com-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpcensus-com/openapi/mcpcensus-com-server-api-openapi.yml
- filename: mcpcensus-com-stats-api-openapi.yml
  format: yaml
  label: MCP Census Stats API
  slug: mcpcensus-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpcensus-com/openapi/mcpcensus-com-stats-api-openapi.yml
- filename: mcpcensus-com-watch-api-openapi.yml
  format: yaml
  label: MCP Census Watch API
  slug: mcpcensus-com-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpcensus-com/openapi/mcpcensus-com-watch-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MCP Census Authentication
name_suffix: Authentication
oauth_flows: []
overview: MCP Census declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MCP Census
provider_slug: mcpcensus-com
scheme_count: 1
schemes:
- evidence: 'Optional header for higher tiers / watches: `x-api-key: <key>`.'
  header: x-api-key
  location: header
  name: x-api-key
  type: apiKey
slug: mcpcensus-com-authentication
source_filename: mcpcensus-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mcpcensus.com/agent-setup/prompt.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mcpcensus.com/agent-setup/prompt.md\nsources:\n- https://mcpcensus.com/agent-setup/prompt.md\n- https://mcpcensus.com/agent-setup/census-preflight.yml\n- https://mcpcensus.com/agent-setup/changes.md\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: 'Optional header for higher tiers / watches: `x-api-key: <key>`.'\n  location: header\n  header: x-api-key\ndocs: https://mcpcensus.com/agent-setup/prompt.md\n"
source_yaml_url: https://artifacts.apis.io/mcpcensus-com/authentication/mcpcensus-com-authentication.yml
summary_line: 1 scheme
tags:
- MCP
- Census
- Verification
- Public Evidence
---
