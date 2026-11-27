---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: stad-gent-catalog-api-openapi.yml
  format: yaml
  label: Stad Gent Catalog API
  slug: stad-gent-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stad-gent/openapi/stad-gent-catalog-api-openapi.yml
- filename: stad-gent-dataset-api-openapi.yml
  format: yaml
  label: Stad Gent Dataset API
  slug: stad-gent-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stad-gent/openapi/stad-gent-dataset-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Stad Gent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stad Gent secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stad Gent
provider_slug: stad-gent
scheme_count: 1
schemes:
- description: API key to make authenticated requests.
  in: query
  name: apikey
  parameter: apikey
  sources:
  - openapi/stad-gent-openapi.yml
  type: apiKey
slug: stad-gent-authentication
source_filename: stad-gent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/stad-gent-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apikey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key to make authenticated requests.\n  sources:\n  - openapi/stad-gent-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/stad-gent/authentication/stad-gent-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Government
- Open Data
- Belgium
- Smart City
- Municipal
- Datasets
---
