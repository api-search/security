---
anonymous_access: false
api_key_in: []
api_specs:
- filename: geometry-app-openapi-generated.yml
  format: yaml
  label: Geometry API
  slug: geometry-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geometry-app/openapi/_ae-authored/geometry-app-openapi-generated.yml
auth_types: []
description: Authentication methods for Geometry MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Geometry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Geometry declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Geometry
provider_slug: geometry-app
scheme_count: 2
schemes:
- evidence: 'Free URL: Authentication = No Auth.'
  name: No Auth
  type: other
- evidence: With your key https://mcp.geometry.app/mcp?key=YOUR_KEY
  how_to_obtain: Obtain a key from any Developer Portal subscription (metered Free or paid). Append it as ?key=YOUR_KEY.
  location: query
  name: API Key
  type: apiKey
slug: geometry-app-authentication
source_filename: geometry-app-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.geometry.app/quickstart.md
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.geometry.app/quickstart.md\nsources:\n- https://docs.geometry.app/quickstart.md\n- https://docs.geometry.app/quickstart\ndescription: Authentication methods for Geometry MCP\nschemes:\n- type: other\n  name: No Auth\n  evidence: 'Free URL: Authentication = No Auth.'\n- type: apiKey\n  name: API Key\n  evidence: With your key https://mcp.geometry.app/mcp?key=YOUR_KEY\n  location: query\n  how_to_obtain: Obtain a key from any Developer Portal subscription (metered Free or paid). Append it as ?key=YOUR_KEY.\nnote: No OAuth flows are described on the pages.\ndocs: https://docs.geometry.app/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/geometry-app/authentication/geometry-app-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Date
- JSON
- RAG
- Calendar
---
