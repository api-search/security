---
api_key_in:
- header
api_specs:
- filename: companies-house-charges-api-openapi.yml
  format: yaml
  label: Companies House charges API
  slug: companies-house-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-charges-api-openapi.yml
- filename: companies-house-filinghistory-api-openapi.yml
  format: yaml
  label: Companies House filingHistory API
  slug: companies-house-filinghistory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-filinghistory-api-openapi.yml
- filename: companies-house-insolvency-api-openapi.yml
  format: yaml
  label: Companies House insolvency API
  slug: companies-house-insolvency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-insolvency-api-openapi.yml
- filename: companies-house-officerdisqualifications-api-openapi.yml
  format: yaml
  label: Companies House officerDisqualifications API
  slug: companies-house-officerdisqualifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-officerdisqualifications-api-openapi.yml
- filename: companies-house-officers-api-openapi.yml
  format: yaml
  label: Companies House officers API
  slug: companies-house-officers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-officers-api-openapi.yml
- filename: companies-house-personswithsignificantcontrol-api-openapi.yml
  format: yaml
  label: Companies House personsWithSignificantControl API
  slug: companies-house-personswithsignificantcontrol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-personswithsignificantcontrol-api-openapi.yml
- filename: companies-house-registeredofficeaddress-api-openapi.yml
  format: yaml
  label: Companies House registeredOfficeAddress API
  slug: companies-house-registeredofficeaddress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-registeredofficeaddress-api-openapi.yml
- filename: companies-house-search-api-openapi.yml
  format: yaml
  label: Companies House search API
  slug: companies-house-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/openapi/companies-house-search-api-openapi.yml
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
provider_slug: companies-house
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/authentication/companies-house-authentication.yml
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
