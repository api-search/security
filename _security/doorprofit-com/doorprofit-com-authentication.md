---
anonymous_access: false
api_key_in: []
api_specs:
- filename: doorprofit-com-openapi-generated.yml
  format: yaml
  label: doorprofit-com API
  slug: doorprofit-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doorprofit-com/openapi/_ae-authored/doorprofit-com-openapi-generated.yml
auth_types: []
description: Authentication methods for DoorProfit API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: doorprofit-com Authentication
name_suffix: Authentication
oauth_flows: []
overview: doorprofit-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: doorprofit-com
provider_slug: doorprofit-com
scheme_count: 2
schemes:
- evidence: Auth is the `key` query parameter.
  how_to_obtain: Sign up at https://api.doorprofit.com/signup, then copy the key from https://api.doorprofit.com/dashboard.
  location: query
  name: apiKey
  type: apiKey
- evidence: 'OAuth (easiest): add the URL to any OAuth‑capable MCP client. The user logs in to DoorProfit and approves.'
  how_to_obtain: Add the MCP URL to an OAuth‑capable client; the user logs in and approves.
  name: OAuth
  type: oauth2
slug: doorprofit-com-authentication
source_filename: doorprofit-com-authentication.yml
source_heading: Authentication Profile
source_url: https://api.doorprofit.com/signup/
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.doorprofit.com/signup/\nsources:\n- https://api.doorprofit.com/signup/\n- https://api.doorprofit.com/docs.md\ndescription: Authentication methods for DoorProfit API\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: Auth is the `key` query parameter.\n  location: query\n  how_to_obtain: Sign up at https://api.doorprofit.com/signup, then copy the key from https://api.doorprofit.com/dashboard.\n- type: oauth2\n  name: OAuth\n  evidence: 'OAuth (easiest): add the URL to any OAuth‑capable MCP client. The user logs in to DoorProfit and approves.'\n  how_to_obtain: Add the MCP URL to an OAuth‑capable client; the user logs in and approves.\ndocs: https://api.doorprofit.com/signup/\n"
source_yaml_url: https://artifacts.apis.io/doorprofit-com/authentication/doorprofit-com-authentication.yml
summary_line: 2 schemes
tags:
- Crime
- Neighborhood Safety
- Registered Offender Search
- Mobile App
- Real Estate Investment
---
