---
anonymous_access: false
api_key_in: []
api_specs:
- filename: findacopacker-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Find A Co-Packer Enquiry API
  slug: findacopacker-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findacopacker-co-uk/openapi/findacopacker-co-uk-enquiry-api-openapi.yml
- filename: findacopacker-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Find A Co-Packer MCP API
  slug: findacopacker-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findacopacker-co-uk/openapi/findacopacker-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Find A Co-Packer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Find A Co-Packer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Find A Co-Packer
provider_slug: findacopacker-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/findacopacker-co-uk-openapi.json
  type: http
slug: findacopacker-co-uk-authentication
source_filename: findacopacker-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/findacopacker-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/findacopacker-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/findacopacker-co-uk/authentication/findacopacker-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Food
- Manufacturing
- Packaging
- United Kingdom
- B2B
---
