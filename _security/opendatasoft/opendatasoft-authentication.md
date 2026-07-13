---
api_key_in:
- query
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Opendatasoft Explore API v2.1
  slug: opendatasoft-explore-api-v21
  spec_type: OpenAPI
  url: https://public.opendatasoft.com/api/explore/v2.1/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Opendatasoft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opendatasoft secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Opendatasoft
provider_slug: opendatasoft
scheme_count: 1
schemes:
- description: API key to make authenticated requests.
  in: query
  name: apikey
  parameter: apikey
  sources:
  - openapi/opendatasoft-explore-api-v2.1.json
  type: apiKey
slug: opendatasoft-authentication
source_filename: opendatasoft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opendatasoft-explore-api-v2.1.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apikey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key to make authenticated requests.\n  sources:\n  - openapi/opendatasoft-explore-api-v2.1.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendatasoft/refs/heads/main/authentication/opendatasoft-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Open Data
- Datasets
- Public Data
- OData
- REST
- Government
- Cities
---
