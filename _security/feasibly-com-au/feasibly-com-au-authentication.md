---
anonymous_access: false
api_key_in: []
api_specs:
- filename: feasibly-com-au-openapi-generated.yml
  format: yaml
  label: Feasibly API
  slug: feasibly-com-au-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feasibly-com-au/openapi/_ae-authored/feasibly-com-au-openapi-generated.yml
auth_types: []
description: Feasibly uses an API key that can be supplied either as a query parameter or as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Feasibly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Feasibly declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Feasibly
provider_slug: feasibly-com-au
scheme_count: 2
schemes:
- evidence: The key travels inside the MCP URL , so anyone who can read that URL can spend your credits — treat it like a password and keep it out of shared configs, screenshots and screen-shares.
  how_to_obtain: Sign up at app.feasibly.com.au/register; the API key is provided instantly on the dashboard.
  location: query
  name: API Key (query)
  type: apiKey
- evidence: 'Over REST, prefer the Authorization: Bearer header, which keeps the key out of URLs and server logs entirely.'
  header: Authorization
  how_to_obtain: Sign up at app.feasibly.com.au/register; the API key is provided instantly on the dashboard.
  location: header
  name: API Key (header)
  type: http-bearer
slug: feasibly-com-au-authentication
source_filename: feasibly-com-au-authentication.yml
source_heading: Authentication Profile
source_url: https://feasibly.com.au/docs/quickstart/
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://feasibly.com.au/docs/quickstart/\nsources:\n- https://feasibly.com.au/docs/quickstart/\ndescription: Feasibly uses an API key that can be supplied either as a query parameter or as a Bearer token in the Authorization header.\nschemes:\n- type: apiKey\n  name: API Key (query)\n  evidence: The key travels inside the MCP URL , so anyone who can read that URL can spend your credits — treat it like a password and keep it\n    out of shared configs, screenshots and screen-shares.\n  location: query\n  how_to_obtain: Sign up at app.feasibly.com.au/register; the API key is provided instantly on the dashboard.\n- type: http-bearer\n  name: API Key (header)\n  evidence: 'Over REST, prefer the Authorization: Bearer header, which keeps the key out of URLs and server logs entirely.'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up at app.feasibly.com.au/register;\
  \ the API key is provided instantly on the dashboard.\ndocs: https://feasibly.com.au/docs/quickstart/\n"
source_yaml_url: https://artifacts.apis.io/feasibly-com-au/authentication/feasibly-com-au-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Planning
- Real Estate
- Data API
- Australia
---
