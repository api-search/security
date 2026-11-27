---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ishlabs-io-environments-api-openapi.yml
  format: yaml
  label: ish Environments API
  slug: ishlabs-io-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ishlabs-io/openapi/ishlabs-io-environments-api-openapi.yml
- filename: ishlabs-io-events-api-openapi.yml
  format: yaml
  label: ish Events API
  slug: ishlabs-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ishlabs-io/openapi/ishlabs-io-events-api-openapi.yml
- filename: ishlabs-io-people-api-openapi.yml
  format: yaml
  label: ish People API
  slug: ishlabs-io-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ishlabs-io/openapi/ishlabs-io-people-api-openapi.yml
- filename: ishlabs-io-sessions-api-openapi.yml
  format: yaml
  label: ish Sessions API
  slug: ishlabs-io-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ishlabs-io/openapi/ishlabs-io-sessions-api-openapi.yml
- filename: ishlabs-io-tasks-api-openapi.yml
  format: yaml
  label: ish Tasks API
  slug: ishlabs-io-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ishlabs-io/openapi/ishlabs-io-tasks-api-openapi.yml
- filename: ishlabs-io-usage-api-openapi.yml
  format: yaml
  label: ish Usage API
  slug: ishlabs-io-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ishlabs-io/openapi/ishlabs-io-usage-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ish Authentication
name_suffix: Authentication
oauth_flows: []
overview: ish declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ish
provider_slug: ishlabs-io
scheme_count: 1
schemes:
- evidence: 'Every request to the ish API carries a bearer token in the Authorization header:'
  header: Authorization
  how_to_obtain: Mint a workspace API key in the product app under Settings → Developers.
  location: header
  name: Workspace API key
  scopes:
  - sessions:run
  - sessions:read
  - environments:read
  - environments:write
  - tasks:read
  - tasks:write
  - people:read
  - people:write
  - usage:read
  type: http-bearer
slug: ishlabs-io-authentication
source_filename: ishlabs-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ishlabs.io/api/authentication
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ishlabs.io/api/authentication\nsources:\n- https://docs.ishlabs.io/api/authentication\n- https://docs.ishlabs.io/cli/auth\n- https://docs.ishlabs.io/mcp/auth\n- https://docs.ishlabs.io/api/quickstart\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Workspace API key\n  evidence: 'Every request to the ish API carries a bearer token in the Authorization header:'\n  location: header\n  header: Authorization\n  scopes:\n  - sessions:run\n  - sessions:read\n  - environments:read\n  - environments:write\n  - tasks:read\n  - tasks:write\n  - people:read\n  - people:write\n  - usage:read\n  how_to_obtain: Mint a workspace API key in the product app under Settings → Developers.\ndocs: https://docs.ishlabs.io/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/ishlabs-io/authentication/ishlabs-io-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Simulation
- Research
- Design
- Platform
---
