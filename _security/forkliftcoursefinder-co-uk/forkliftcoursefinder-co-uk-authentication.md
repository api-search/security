---
anonymous_access: false
api_key_in: []
api_specs:
- filename: forkliftcoursefinder-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Forklift Course Finder Enquiry API
  slug: forkliftcoursefinder-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forkliftcoursefinder-co-uk/openapi/forkliftcoursefinder-co-uk-enquiry-api-openapi.yml
- filename: forkliftcoursefinder-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Forklift Course Finder MCP API
  slug: forkliftcoursefinder-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forkliftcoursefinder-co-uk/openapi/forkliftcoursefinder-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Forklift Course Finder Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forklift Course Finder secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Forklift Course Finder
provider_slug: forkliftcoursefinder-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/forkliftcoursefinder-co-uk-openapi.json
  type: http
slug: forkliftcoursefinder-co-uk-authentication
source_filename: forkliftcoursefinder-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/forkliftcoursefinder-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/forkliftcoursefinder-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/forkliftcoursefinder-co-uk/authentication/forkliftcoursefinder-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Forklift
- Training
- United Kingdom
- HSE
- Data
---
