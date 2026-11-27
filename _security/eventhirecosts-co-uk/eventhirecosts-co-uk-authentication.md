---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eventhirecosts-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Event Hire Costs Enquiry API
  slug: eventhirecosts-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eventhirecosts-co-uk/openapi/eventhirecosts-co-uk-enquiry-api-openapi.yml
- filename: eventhirecosts-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Event Hire Costs MCP API
  slug: eventhirecosts-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eventhirecosts-co-uk/openapi/eventhirecosts-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Event Hire Costs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Event Hire Costs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Event Hire Costs
provider_slug: eventhirecosts-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/eventhirecosts-co-uk-openapi.json
  type: http
slug: eventhirecosts-co-uk-authentication
source_filename: eventhirecosts-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/eventhirecosts-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/eventhirecosts-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/eventhirecosts-co-uk/authentication/eventhirecosts-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Event
- Hire
- Costs
- United Kingdom
- Quotes
---
