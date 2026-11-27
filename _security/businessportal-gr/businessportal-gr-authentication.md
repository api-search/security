---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: businessportal-gr-companies-api-openapi.yml
  format: yaml
  label: GEMI General Commercial Registry (Greece) Companies API
  slug: businessportal-gr-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessportal-gr/openapi/businessportal-gr-companies-api-openapi.yml
- filename: businessportal-gr-companydocuments-api-openapi.yml
  format: yaml
  label: GEMI General Commercial Registry (Greece) Company Documents API
  slug: businessportal-gr-companydocuments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessportal-gr/openapi/businessportal-gr-companydocuments-api-openapi.yml
- filename: businessportal-gr-downloadfile-api-openapi.yml
  format: yaml
  label: GEMI General Commercial Registry (Greece) Download File API
  slug: businessportal-gr-downloadfile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessportal-gr/openapi/businessportal-gr-downloadfile-api-openapi.yml
- filename: businessportal-gr-metadata-api-openapi.yml
  format: yaml
  label: GEMI General Commercial Registry (Greece) Metadata API
  slug: businessportal-gr-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessportal-gr/openapi/businessportal-gr-metadata-api-openapi.yml
- filename: businessportal-gr-misc-api-openapi.yml
  format: yaml
  label: GEMI General Commercial Registry (Greece) Misc API
  slug: businessportal-gr-misc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessportal-gr/openapi/businessportal-gr-misc-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: GEMI General Commercial Registry (Greece) Authentication
name_suffix: Authentication
oauth_flows: []
overview: GEMI General Commercial Registry (Greece) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GEMI General Commercial Registry (Greece)
provider_slug: businessportal-gr
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: api_key
  sources:
  - openapi/businessportal-gr-openapi.yml
  type: apiKey
slug: businessportal-gr-authentication
source_filename: businessportal-gr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/businessportal-gr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: api_key\n  sources:\n  - openapi/businessportal-gr-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/businessportal-gr/authentication/businessportal-gr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Business Registry
- Government
- Open Data
- Greece
- Company Data
- Public Sector
---
