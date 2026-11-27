---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gallbladdersurgerycost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Gallbladder Surgery Cost Enquiry API
  slug: gallbladdersurgerycost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gallbladdersurgerycost-co-uk/openapi/gallbladdersurgerycost-co-uk-enquiry-api-openapi.yml
- filename: gallbladdersurgerycost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Gallbladder Surgery Cost MCP API
  slug: gallbladdersurgerycost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gallbladdersurgerycost-co-uk/openapi/gallbladdersurgerycost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Gallbladder Surgery Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gallbladder Surgery Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gallbladder Surgery Cost
provider_slug: gallbladdersurgerycost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/gallbladdersurgerycost-co-uk-openapi.json
  type: http
slug: gallbladdersurgerycost-co-uk-authentication
source_filename: gallbladdersurgerycost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/gallbladdersurgerycost-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/gallbladdersurgerycost-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/gallbladdersurgerycost-co-uk/authentication/gallbladdersurgerycost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- United Kingdom
- Surgery
- Pricing
- Medical
---
