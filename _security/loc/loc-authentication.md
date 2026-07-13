---
api_key_in:
- query
api_specs:
- filename: loc-loc-gov-json-api-openapi.yml
  format: yaml
  label: loc.gov JSON API
  slug: locgov-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loc/refs/heads/main/openapi/loc-loc-gov-json-api-openapi.yml
- filename: loc-congress-gov-openapi.yml
  format: yaml
  label: Congress.gov API
  slug: congressgov-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loc/refs/heads/main/openapi/loc-congress-gov-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Loc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Library of Congress secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Library of Congress
provider_slug: loc
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/loc-congress-gov-openapi.yml
  type: apiKey
slug: loc-authentication
source_filename: loc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/loc-congress-gov-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/loc-congress-gov-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loc/refs/heads/main/authentication/loc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Library
- Government
- Congress
- Legislative Data
- Digital Collections
- Newspapers
- Maps
- Bibliographic Records
- Historical Documents
---
