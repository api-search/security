---
anonymous_access: false
api_key_in: []
api_specs:
- filename: beecargo-net-agent-api-openapi.yml
  format: yaml
  label: Beecargo Agent API
  slug: beecargo-net-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beecargo-net/openapi/beecargo-net-agent-api-openapi.yml
- filename: beecargo-net-connect-api-openapi.yml
  format: yaml
  label: Beecargo Connect API
  slug: beecargo-net-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beecargo-net/openapi/beecargo-net-connect-api-openapi.yml
- filename: beecargo-net-downloads-api-openapi.yml
  format: yaml
  label: Beecargo Downloads API
  slug: beecargo-net-downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beecargo-net/openapi/beecargo-net-downloads-api-openapi.yml
- filename: beecargo-net-files-api-openapi.yml
  format: yaml
  label: Beecargo Files API
  slug: beecargo-net-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beecargo-net/openapi/beecargo-net-files-api-openapi.yml
- filename: beecargo-net-folders-api-openapi.yml
  format: yaml
  label: Beecargo Folders API
  slug: beecargo-net-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beecargo-net/openapi/beecargo-net-folders-api-openapi.yml
- filename: beecargo-net-system-api-openapi.yml
  format: yaml
  label: Beecargo System API
  slug: beecargo-net-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beecargo-net/openapi/beecargo-net-system-api-openapi.yml
auth_types: []
description: Authentication methods as published on the page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Beecargo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beecargo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Beecargo
provider_slug: beecargo-net
scheme_count: 1
schemes:
- evidence: Call beecargo_register_agent to get an API key (upload access, free-tier quotas).
  how_to_obtain: Call beecargo_register_agent to get an API key (upload access, free-tier quotas).
  name: API key
  type: apiKey
slug: beecargo-net-authentication
source_filename: beecargo-net-authentication.yml
source_heading: Authentication Profile
source_url: https://beecargo.net/agents/mcp-quickstart
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://beecargo.net/agents/mcp-quickstart\nsources:\n- https://beecargo.net/agents/mcp-quickstart\ndescription: Authentication methods as published on the page.\nschemes:\n- type: apiKey\n  name: API key\n  evidence: Call beecargo_register_agent to get an API key (upload access, free-tier quotas).\n  how_to_obtain: Call beecargo_register_agent to get an API key (upload access, free-tier quotas).\ndocs: https://beecargo.net/agents/mcp-quickstart\n"
source_yaml_url: https://artifacts.apis.io/beecargo-net/authentication/beecargo-net-authentication.yml
summary_line: 1 scheme
tags:
- File Hosting
- Share Links
- Developers
- Agents
---
