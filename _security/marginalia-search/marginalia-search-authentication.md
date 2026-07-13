---
api_key_in:
- header
api_specs:
- filename: marginalia-search-openapi.yml
  format: yaml
  label: Marginalia Search API
  slug: marginalia-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marginalia-search/refs/heads/main/openapi/marginalia-search-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Marginalia Search Authentication
name_suffix: Authentication
oauth_flows: []
overview: Marginalia Search secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Marginalia Search
provider_slug: marginalia-search
scheme_count: 1
schemes:
- description: API key supplied via the API-Key header. A public testing key is documented; commercial and non-commercial keys are issued by contact@marginalia-search.com or via Polar.
  in: header
  name: APIKey
  parameter: API-Key
  sources:
  - openapi/marginalia-search-openapi.yml
  type: apiKey
slug: marginalia-search-authentication
source_filename: marginalia-search-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/marginalia-search-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: API-Key\n  description: API key supplied via the API-Key header. A public testing key is documented;\n    commercial and non-commercial keys are issued by contact@marginalia-search.com or via Polar.\n  sources:\n  - openapi/marginalia-search-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marginalia-search/refs/heads/main/authentication/marginalia-search-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Open Source
- Search
- Web Search
---
