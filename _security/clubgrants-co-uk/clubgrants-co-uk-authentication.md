---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clubgrants-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Club Grants Enquiry API
  slug: clubgrants-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clubgrants-co-uk/openapi/clubgrants-co-uk-enquiry-api-openapi.yml
- filename: clubgrants-co-uk-guide-api-openapi.yml
  format: yaml
  label: Club Grants Guide API
  slug: clubgrants-co-uk-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clubgrants-co-uk/openapi/clubgrants-co-uk-guide-api-openapi.yml
- filename: clubgrants-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Club Grants MCP API
  slug: clubgrants-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clubgrants-co-uk/openapi/clubgrants-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Club Grants Authentication
name_suffix: Authentication
oauth_flows: []
overview: Club Grants secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Club Grants
provider_slug: clubgrants-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  key_prefix: emk_
  name: accessKey
  required: false
  scheme: bearer
  sources:
  - openapi/clubgrants-co-uk-openapi.yml
  type: http
slug: clubgrants-co-uk-authentication
source_filename: clubgrants-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clubgrants.co.uk/mcp\ndocs: https://clubgrants.co.uk/mcp\nsummary:\n  types:\n  - http\n  optional: true\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  key_prefix: emk_\n  required: false\n  sources:\n  - openapi/clubgrants-co-uk-openapi.yml\nnote: 'Every tool operation in the OpenAPI declares security [{}, {accessKey: []}], i.e. anonymous OR bearer access key. The MCP server card served at GET https://clubgrants.co.uk/mcp (HTTP 200, fetched 2026-11-04) states \"auth\": \"none\" for the MCP endpoint. No page documenting how an emk_ key is obtained was found; the spec''s 429 description cites docs/MCP.md, which returned HTTP 404 at https://clubgrants.co.uk/docs/MCP.md.'\n"
source_yaml_url: https://artifacts.apis.io/clubgrants-co-uk/authentication/clubgrants-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Grants
- Funding
- Sports
- Non-Profit
- Open Data
- United Kingdom
- MCP
---
