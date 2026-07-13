---
api_key_in:
- header
api_specs:
- filename: sigma-aldrich-product-openapi.yml
  format: yaml
  label: Sigma-Aldrich Product Search API
  slug: sigma-aldrich-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sigma-aldrich/refs/heads/main/openapi/sigma-aldrich-product-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sigma Aldrich Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sigma-Aldrich secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sigma-Aldrich
provider_slug: sigma-aldrich
scheme_count: 1
schemes:
- description: Sigma-Aldrich API key for authentication
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/sigma-aldrich-product-openapi.yml
  type: apiKey
slug: sigma-aldrich-authentication
source_filename: sigma-aldrich-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sigma-aldrich-product-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Sigma-Aldrich API key for authentication\n  sources:\n  - openapi/sigma-aldrich-product-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sigma-aldrich/refs/heads/main/authentication/sigma-aldrich-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Life Science
- Chemistry
- Biochemistry
- Laboratory
- Research
- Chemical Catalog
---
