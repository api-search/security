---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dilapidationsquotes-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Dilapidations Quotes Enquiry API
  slug: dilapidationsquotes-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dilapidationsquotes-co-uk/openapi/dilapidationsquotes-co-uk-enquiry-api-openapi.yml
- filename: dilapidationsquotes-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Dilapidations Quotes MCP API
  slug: dilapidationsquotes-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dilapidationsquotes-co-uk/openapi/dilapidationsquotes-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dilapidationsquotes Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dilapidations Quotes secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dilapidations Quotes
provider_slug: dilapidationsquotes-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/dilapidationsquotes-co-uk-openapi.yml
  type: http
slug: dilapidationsquotes-co-uk-authentication
source_filename: dilapidationsquotes-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://dilapidationsquotes.co.uk/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with\n    it; the bulk entity export requires one.'\n  sources:\n  - openapi/dilapidationsquotes-co-uk-openapi.yml\ndocs: https://dilapidationsquotes.co.uk/mcp\noptional: true\nnotes: 'Every operation declares security [{}, {accessKey: []}]: unauthenticated calls\n  are allowed on a free tier and an optional bearer access key (emk_...) raises the\n  budget. The provider-hosted MCP card (GET https://dilapidationsquotes.co.uk/mcp,\n  HTTP 200) states \"auth\": \"none\" for the MCP endpoint. No page documenting how to\n  obtain an access key was found; the spec''s 429 text references docs/MCP.md, which\n  returned HTTP 404 at https://dilapidationsquotes.co.uk/docs/MCP.md on 2026-11-05.'\n"
source_yaml_url: https://artifacts.apis.io/dilapidationsquotes-co-uk/authentication/dilapidationsquotes-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Dilapidations
- Commercial Property
- Property Law
- Surveying
- Landlord and Tenant
- United Kingdom
- Quotes
---
