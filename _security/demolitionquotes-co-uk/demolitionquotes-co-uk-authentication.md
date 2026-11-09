---
anonymous_access: true
api_key_in: []
api_specs:
- filename: demolitionquotes-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Demolition Quotes Enquiry API
  slug: demolitionquotes-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/demolitionquotes-co-uk/openapi/demolitionquotes-co-uk-enquiry-api-openapi.yml
- filename: demolitionquotes-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Demolition Quotes MCP API
  slug: demolitionquotes-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/demolitionquotes-co-uk/openapi/demolitionquotes-co-uk-mcp-api-openapi.yml
auth_types:
- http
- none
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Demolitionquotes Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Demolition Quotes secures its APIs with http and none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Demolition Quotes
provider_slug: demolitionquotes-co-uk
scheme_count: 2
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  optional: true
  scheme: bearer
  sources:
  - openapi/demolitionquotes-co-uk-openapi.yml
  type: http
- description: The MCP server card at https://demolitionquotes.co.uk/mcp declares "auth":"none" for the streamable-http MCP endpoint; calls work without a key up to the free tier (429 past it).
  name: none
  sources:
  - https://demolitionquotes.co.uk/mcp
  type: none
slug: demolitionquotes-co-uk-authentication
source_filename: demolitionquotes-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://demolitionquotes.co.uk/mcp\ndocs: https://demolitionquotes.co.uk/mcp\nsummary:\n  types:\n  - http\n  - none\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  optional: true\n  sources:\n  - openapi/demolitionquotes-co-uk-openapi.yml\n- name: none\n  type: none\n  description: The MCP server card at https://demolitionquotes.co.uk/mcp declares \"auth\":\"none\" for the\n    streamable-http MCP endpoint; calls work without a key up to the free tier (429 past it).\n  sources:\n  - https://demolitionquotes.co.uk/mcp\nnote: The spec declares accessKey in components but sets no global security requirement. No page\n  documents how to obtain an emk_ key (the docs/MCP.md referenced in 429 descriptions returned 404 on 2026-11-05).\n"
source_yaml_url: https://artifacts.apis.io/demolitionquotes-co-uk/authentication/demolitionquotes-co-uk-authentication.yml
summary_line: http/none · 2 schemes
tags:
- Company
- Demolition
- Construction
- Quotes
- Cost Calculator
- United Kingdom
- Lead Generation
---
