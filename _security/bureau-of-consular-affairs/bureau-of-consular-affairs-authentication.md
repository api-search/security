---
api_key_in:
- header
api_specs:
- filename: bureau-of-consular-affairs-openapi.yml
  format: yaml
  label: Bureau of Consular Affairs Data Catalog (CKAN API)
  slug: ca-data-catalog-ckan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-consular-affairs/refs/heads/main/openapi/bureau-of-consular-affairs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bureau Of Consular Affairs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bureau of Consular Affairs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bureau of Consular Affairs
provider_slug: bureau-of-consular-affairs
scheme_count: 1
schemes:
- description: CKAN API token, generated from the CKAN user profile.
  in: header
  name: apiToken
  parameter: Authorization
  sources:
  - openapi/bureau-of-consular-affairs-openapi.yml
  type: apiKey
slug: bureau-of-consular-affairs-authentication
source_filename: bureau-of-consular-affairs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bureau-of-consular-affairs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: CKAN API token, generated from the CKAN user profile.\n  sources:\n  - openapi/bureau-of-consular-affairs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-consular-affairs/refs/heads/main/authentication/bureau-of-consular-affairs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federal Government
- Passports
- Travel
- Travel Advisories
- Visas
---
