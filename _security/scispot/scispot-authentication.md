---
api_key_in:
- header
api_specs:
- filename: scispot-eln-api-openapi.yml
  format: yaml
  label: Scispot ELN API
  slug: scispot-eln-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scispot/refs/heads/main/openapi/scispot-eln-api-openapi.yml
- filename: scispot-labsheets-api-openapi.yml
  format: yaml
  label: Scispot Labsheets API
  slug: scispot-labsheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scispot/refs/heads/main/openapi/scispot-labsheets-api-openapi.yml
- filename: scispot-manifests-api-openapi.yml
  format: yaml
  label: Scispot Manifests API
  slug: scispot-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scispot/refs/heads/main/openapi/scispot-manifests-api-openapi.yml
- filename: scispot-samples-api-openapi.yml
  format: yaml
  label: Scispot Samples API
  slug: scispot-samples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scispot/refs/heads/main/openapi/scispot-samples-api-openapi.yml
- filename: scispot-sequences-api-openapi.yml
  format: yaml
  label: Scispot Sequences API
  slug: scispot-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scispot/refs/heads/main/openapi/scispot-sequences-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Scispot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scispot secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scispot
provider_slug: scispot
scheme_count: 1
schemes:
- description: Personal API token generated from Scispot Account Settings > Personal Tokens. All API requests require this header.
  in: header
  name: ApiKeyAuth
  parameter: apiKey
  sources:
  - openapi/scispot-openapi.yml
  type: apiKey
slug: scispot-authentication
source_filename: scispot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scispot-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: Personal API token generated from Scispot Account Settings > Personal Tokens.\n    All API requests require this header.\n  sources:\n  - openapi/scispot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scispot/refs/heads/main/authentication/scispot-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Laboratory
- Life Science
- LIMS
- ELN
- Biotech
- API-First
- Scientific Data
- Healthcare
---
