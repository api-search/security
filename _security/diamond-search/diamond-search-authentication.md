---
api_key_in:
- header
api_specs:
- filename: idex-onsite-full-feed-api-openapi.yml
  format: yaml
  label: IDEX Onsite Full Feed API
  slug: idex-onsite-full-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diamond-search/refs/heads/main/openapi/idex-onsite-full-feed-api-openapi.yml
- filename: idex-lab-grown-file-api-openapi.yml
  format: yaml
  label: IDEX Lab Grown File API
  slug: idex-lab-grown-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diamond-search/refs/heads/main/openapi/idex-lab-grown-file-api-openapi.yml
- filename: idex-data-report-api-openapi.yml
  format: yaml
  label: IDEX Data Report API
  slug: idex-data-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diamond-search/refs/heads/main/openapi/idex-data-report-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Diamond Search Authentication
name_suffix: Authentication
oauth_flows: []
overview: Diamond Search secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Diamond Search
provider_slug: diamond-search
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/idex-lab-grown-file-api-openapi.yml
  type: apiKey
slug: diamond-search-authentication
source_filename: diamond-search-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/idex-lab-grown-file-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/idex-lab-grown-file-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diamond-search/refs/heads/main/authentication/diamond-search-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Diamonds
- Lab Grown
- Pricing
- Trading
---
