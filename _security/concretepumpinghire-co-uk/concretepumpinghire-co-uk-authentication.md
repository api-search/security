---
anonymous_access: false
api_key_in: []
api_specs:
- filename: concretepumpinghire-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Concrete Pumping Hire Enquiry API
  slug: concretepumpinghire-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concretepumpinghire-co-uk/openapi/concretepumpinghire-co-uk-enquiry-api-openapi.yml
- filename: concretepumpinghire-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Concrete Pumping Hire MCP API
  slug: concretepumpinghire-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/concretepumpinghire-co-uk/openapi/concretepumpinghire-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Concrete Pumping Hire Authentication
name_suffix: Authentication
oauth_flows: []
overview: Concrete Pumping Hire secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Concrete Pumping Hire
provider_slug: concretepumpinghire-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/concretepumpinghire-co-uk-openapi.yml
  type: http
slug: concretepumpinghire-co-uk-authentication
source_filename: concretepumpinghire-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/concretepumpinghire-co-uk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/concretepumpinghire-co-uk-openapi.yml\noptional: true\nnote: 'Every tool operation declares security [{}, {accessKey: []}], so the bearer access key is optional; the MCP card at https://concretepumpinghire.co.uk/mcp (GET 200, 2026-11-04) states \"auth\": \"none\". The 429 response reads \"Past the free tier for this caller; an access key raises the ceiling (docs/MCP.md)\". No docs page describing how to obtain an emk_ key was found.'\n"
source_yaml_url: https://artifacts.apis.io/concretepumpinghire-co-uk/authentication/concretepumpinghire-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Construction
- Concrete Pumping
- Equipment Hire
- Lead Generation
- United Kingdom
- Datasets
---
