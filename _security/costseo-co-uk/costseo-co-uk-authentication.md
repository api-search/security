---
anonymous_access: false
api_key_in: []
api_specs:
- filename: costseo-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Cost SEO Enquiry API
  slug: costseo-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costseo-co-uk/openapi/costseo-co-uk-enquiry-api-openapi.yml
- filename: costseo-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Cost SEO MCP API
  slug: costseo-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/costseo-co-uk/openapi/costseo-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cost SEO Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cost SEO secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cost SEO
provider_slug: costseo-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  key_prefix: emk_
  name: accessKey
  required: false
  scheme: bearer
  sources:
  - openapi/costseo-co-uk-openapi.yml
  - https://costseo.co.uk/mcp
  type: http
slug: costseo-co-uk-authentication
source_filename: costseo-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://costseo.co.uk/mcp\ndocs: https://costseo.co.uk/mcp\nsummary:\n  types:\n  - http\n  optional: true\n  note: 'The MCP server card served at GET https://costseo.co.uk/mcp (HTTP 200) declares \"auth\": \"none\"; the OpenAPI describes an optional bearer access key that raises the free-tier ceiling.'\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  key_prefix: emk_\n  required: false\n  sources:\n  - openapi/costseo-co-uk-openapi.yml\n  - https://costseo.co.uk/mcp\n"
source_yaml_url: https://artifacts.apis.io/costseo-co-uk/authentication/costseo-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- SEO
- Pricing Data
- Marketing
- United Kingdom
- MCP
- Datasets
---
