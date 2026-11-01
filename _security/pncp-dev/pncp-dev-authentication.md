---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pncp-dev-openapi-generated.yml
  format: yaml
  label: pncp-dev API
  slug: pncp-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pncp-dev/openapi/_ae-authored/pncp-dev-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Pncp Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: pncp-dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: pncp-dev
provider_slug: pncp-dev
scheme_count: 2
schemes:
- description: API key provided in the x-api-key header.
  in: header
  name: x-api-key
  type: apiKey
- description: API key can also be passed as api_key query parameter.
  in: query
  name: api_key
  type: apiKey
slug: pncp-dev-authentication
source_filename: pncp-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://pncp.dev/docs#chave\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: API key provided in the x-api-key header.\n  - type: apiKey\n    name: api_key\n    in: query\n    description: API key can also be passed as api_key query parameter.\n"
source_yaml_url: https://artifacts.apis.io/pncp-dev/authentication/pncp-dev-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API Proxy
- Public Data
- Brazil
- Procurement
- Open Data
---
