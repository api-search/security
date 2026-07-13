---
api_key_in: []
api_specs:
- filename: zenodo-rest-api-openapi.yml
  format: yaml
  label: Zenodo REST API
  slug: zenodo-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenodo/refs/heads/main/openapi/zenodo-rest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zenodo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zenodo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zenodo
provider_slug: zenodo
scheme_count: 1
schemes:
- description: Personal access token issued from the Zenodo account settings
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/zenodo-rest-api-openapi.yml
  type: http
slug: zenodo-authentication
source_filename: zenodo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zenodo-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Personal access token issued from the Zenodo account settings\n  sources:\n  - openapi/zenodo-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenodo/refs/heads/main/authentication/zenodo-authentication.yml
summary_line: http · 1 scheme
tags:
- Research
- Open Data
- Repository
- DOI
- Datasets
- Software
- CERN
- OpenAIRE
- InvenioRDM
- Open Science
- Metadata
- Harvesting
---
