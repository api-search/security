---
anonymous_access: true
api_key_in: []
api_specs:
- filename: copywritingseo-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Copywriting for SEO Enquiry API
  slug: copywritingseo-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/copywritingseo-co-uk/openapi/copywritingseo-co-uk-enquiry-api-openapi.yml
- filename: copywritingseo-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Copywriting for SEO MCP API
  slug: copywritingseo-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/copywritingseo-co-uk/openapi/copywritingseo-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Copywriting for SEO Authentication
name_suffix: Authentication
oauth_flows: []
overview: Copywriting for SEO secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Copywriting for SEO
provider_slug: copywritingseo-co-uk
scheme_count: 2
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  required: false
  scheme: bearer
  sources:
  - openapi/copywritingseo-co-uk-openapi.yml
  type: http
- description: MCP card states "auth":"none" for the Streamable HTTP endpoint https://copywritingseo.co.uk/mcp.
  name: none
  sources:
  - https://copywritingseo.co.uk/mcp
  type: none
slug: copywritingseo-co-uk-authentication
source_filename: copywritingseo-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://copywritingseo.co.uk/mcp\ndocs: https://copywritingseo.co.uk/mcp\nsummary:\n  types:\n  - http\n  anonymous_access: true\n  note: The MCP card at https://copywritingseo.co.uk/mcp (HTTP 200, fetched 2026-11-04) declares \"auth\":\"none\"; the OpenAPI\n    declares an optional bearer access key (emk_...) that raises the caller's budget above the free tier.\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  required: false\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'\n  sources:\n  - openapi/copywritingseo-co-uk-openapi.yml\n- name: none\n  type: none\n  description: MCP card states \"auth\":\"none\" for the Streamable HTTP endpoint https://copywritingseo.co.uk/mcp.\n  sources:\n  - https://copywritingseo.co.uk/mcp\n"
source_yaml_url: https://artifacts.apis.io/copywritingseo-co-uk/authentication/copywritingseo-co-uk-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Copywriting
- SEO
- Content Writing
- Marketing
- Pricing Data
- United Kingdom
---
