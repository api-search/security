---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Country Calling Codes API
  slug: country-calling-codes-api
  spec_type: OpenAPI
  url: https://www.countrycalling.codes/api/calling-codes/openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Country Calling Codes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Country Calling Codes declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Country Calling Codes
provider_slug: country-calling-codes
scheme_count: 0
schemes: []
slug: country-calling-codes-authentication
source_filename: country-calling-codes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: >-\n  openapi/country-calling-codes-openapi.json (empty security/securitySchemes) +\n  https://www.countrycalling.codes/developers + llms.txt + live anonymous probes\n  of the REST and MCP surfaces (2026-09-09).\ndocs: https://www.countrycalling.codes/developers\nprofile:\n  authentication: none\n  api_key_required: false\n  oauth: false\n  notes: >-\n    Deliberately open: the OpenAPI declares security: [] with no securitySchemes,\n    the info.description states \"No authentication is required\", and anonymous\n    probes of GET /api/calling-codes/US, GET /api/capabilities, and the MCP\n    endpoint (initialize + tools/list) all succeeded with no credentials. The MCP\n    Registry manifest declares authentication: none and readOnly: true. CORS\n    allows cross-origin GET from any origin (access-control-allow-origin: *).\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/country-calling-codes/refs/heads/main/authentication/country-calling-codes-authentication.yml
summary_line: 0 schemes
tags:
- data
- reference
- telecom
- phone
- openapi
- mcp
---
