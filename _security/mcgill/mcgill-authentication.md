---
api_key_in:
- header
api_specs:
- filename: mcgill-dataverses-api-openapi.yml
  format: yaml
  label: McGill University Dataverses API
  slug: mcgill-dataverses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/openapi/mcgill-dataverses-api-openapi.yml
- filename: mcgill-info-api-openapi.yml
  format: yaml
  label: McGill University Info API
  slug: mcgill-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/openapi/mcgill-info-api-openapi.yml
- filename: mcgill-search-api-openapi.yml
  format: yaml
  label: McGill University Search API
  slug: mcgill-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/openapi/mcgill-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mcgill Authentication
name_suffix: Authentication
oauth_flows: []
overview: McGill University secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: McGill University
provider_slug: mcgill
scheme_count: 1
schemes:
- description: Dataverse API token, required for write/admin and private-data operations.
  in: header
  name: ApiKeyAuth
  parameter: X-Dataverse-key
  sources:
  - openapi/mcgill-dataverse-native.yaml
  type: apiKey
slug: mcgill-authentication
source_filename: mcgill-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mcgill-dataverse-native.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Dataverse-key\n  description: Dataverse API token, required for write/admin and private-data operations.\n  sources:\n  - openapi/mcgill-dataverse-native.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/authentication/mcgill-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- Canada
- Quebec
---
