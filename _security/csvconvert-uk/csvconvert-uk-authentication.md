---
anonymous_access: false
api_key_in: []
api_specs:
- filename: csvconvert-uk-enquiry-api-openapi.yml
  format: yaml
  label: CSV Convert Enquiry API
  slug: csvconvert-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csvconvert-uk/openapi/csvconvert-uk-enquiry-api-openapi.yml
- filename: csvconvert-uk-guide-api-openapi.yml
  format: yaml
  label: CSV Convert Guide API
  slug: csvconvert-uk-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csvconvert-uk/openapi/csvconvert-uk-guide-api-openapi.yml
- filename: csvconvert-uk-mcp-api-openapi.yml
  format: yaml
  label: CSV Convert MCP API
  slug: csvconvert-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csvconvert-uk/openapi/csvconvert-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: CSV Convert Authentication
name_suffix: Authentication
oauth_flows: []
overview: CSV Convert secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CSV Convert
provider_slug: csvconvert-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/csvconvert-uk-openapi.yml
  type: http
slug: csvconvert-uk-authentication
source_filename: csvconvert-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/csvconvert-uk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/csvconvert-uk-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/csvconvert-uk/authentication/csvconvert-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- CSV
- PDF
- Data Conversion
- Data Extraction
- OCR
- United Kingdom
- Data Protection
---
