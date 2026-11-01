---
anonymous_access: false
api_key_in: []
api_specs:
- filename: worthune-openapi-generated.yml
  format: yaml
  label: Worthune API
  slug: worthune-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/worthune/openapi/_ae-authored/worthune-openapi-generated.yml
auth_types: []
description: Authentication for Worthune API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Worthune Authentication
name_suffix: Authentication
oauth_flows: []
overview: Worthune declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Worthune
provider_slug: worthune
scheme_count: 3
schemes:
- evidence: 'Paid calls authenticate with Authorization: Bearer wk_…'
  header: Authorization
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'Paid calls authenticate with Authorization: Bearer wk_… (or an x-api-key header; the MCP run_model tool takes an api_key argument).'
  header: x-api-key
  location: header
  name: x-api-key header
  type: apiKey
- evidence: the MCP run_model tool takes an api_key argument
  location: query
  name: api_key query/body argument
  type: apiKey
slug: worthune-authentication
source_filename: worthune-authentication.yml
source_heading: Authentication Profile
source_url: https://worthune.com/docs
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://worthune.com/docs\nsources:\n- https://worthune.com/docs\ndescription: Authentication for Worthune API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Paid calls authenticate with Authorization: Bearer wk_…'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: x-api-key header\n  evidence: 'Paid calls authenticate with Authorization: Bearer wk_… (or an x-api-key header; the MCP run_model tool takes an api_key argument).'\n  location: header\n  header: x-api-key\n- type: apiKey\n  name: api_key query/body argument\n  evidence: the MCP run_model tool takes an api_key argument\n  location: query\nnote: No OAuth flows are described on the page.\ndocs: https://worthune.com/docs\n"
source_yaml_url: https://artifacts.apis.io/worthune/authentication/worthune-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Finance
- WealthTech
- Platform
---
