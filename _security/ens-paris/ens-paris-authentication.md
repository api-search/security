---
api_key_in:
- query
api_specs:
- filename: ens-paris-mesr-opendata.yaml
  format: yaml
  label: MESR Higher Education Open Data (Explore API)
  slug: mesr-opendata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ens-paris/refs/heads/main/openapi/ens-paris-mesr-opendata.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ens Paris Authentication
name_suffix: Authentication
oauth_flows: []
overview: École Normale Supérieure de Paris secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: École Normale Supérieure de Paris
provider_slug: ens-paris
scheme_count: 1
schemes:
- description: API key to make authenticated requests.
  in: query
  name: apikey
  parameter: apikey
  sources:
  - openapi/ens-paris-mesr-opendata.yaml
  type: apiKey
slug: ens-paris-authentication
source_filename: ens-paris-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ens-paris-mesr-opendata.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apikey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key to make authenticated requests.\n  sources:\n  - openapi/ens-paris-mesr-opendata.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ens-paris/refs/heads/main/authentication/ens-paris-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Open Access
- France
---
