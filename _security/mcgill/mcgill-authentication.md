---
api_key_in:
- header
api_specs:
- filename: mcgill-dataverse-native.yaml
  format: yaml
  label: McGill University Dataverse (Borealis) - Native API
  slug: dataverse-native
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/openapi/mcgill-dataverse-native.yaml
- filename: mcgill-dataverse-search.yaml
  format: yaml
  label: McGill University Dataverse (Borealis) - Search API
  slug: dataverse-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/openapi/mcgill-dataverse-search.yaml
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
