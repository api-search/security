---
api_key_in:
- header
api_specs:
- filename: specs.developer.ch.gov.uk
  format: yaml
  label: Companies House Public Data API
  slug: companies-house-public-data-api
  spec_type: OpenAPI
  url: https://github.com/companieshouse/specs.developer.ch.gov.uk
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Companies House Authentication
name_suffix: Authentication
oauth_flows: []
overview: Companies House secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Companies House
provider_slug: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/apis.yml
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: api_key
  sources:
  - openapi/companies-house-public-data-openapi.yml
  type: apiKey
slug: companies-house-authentication
source_filename: companies-house-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/companies-house-public-data-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: api_key\n  sources:\n  - openapi/companies-house-public-data-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/apis.yml/refs/heads/main/authentication/companies-house-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Companies
- UK Government
- Business Registration
- Company Search
- Officers
- Filing History
- Insolvency
- Charges
- Persons of Significant Control
- Open Data
---
