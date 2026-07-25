---
api_key_in: []
api_specs:
- filename: university-of-amsterdam-accounts-api-openapi.yml
  format: yaml
  label: University of Amsterdam Accounts API
  slug: university-of-amsterdam-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-accounts-api-openapi.yml
- filename: university-of-amsterdam-assets-api-openapi.yml
  format: yaml
  label: University of Amsterdam Assets API
  slug: university-of-amsterdam-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-assets-api-openapi.yml
- filename: university-of-amsterdam-datasets-api-openapi.yml
  format: yaml
  label: University of Amsterdam Datasets API
  slug: university-of-amsterdam-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-datasets-api-openapi.yml
- filename: university-of-amsterdam-graphql-api-openapi.yml
  format: yaml
  label: University of Amsterdam GraphQL API
  slug: university-of-amsterdam-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-graphql-api-openapi.yml
- filename: university-of-amsterdam-graphs-api-openapi.yml
  format: yaml
  label: University of Amsterdam Graphs API
  slug: university-of-amsterdam-graphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-graphs-api-openapi.yml
- filename: university-of-amsterdam-hooks-api-openapi.yml
  format: yaml
  label: University of Amsterdam Hooks API
  slug: university-of-amsterdam-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-hooks-api-openapi.yml
- filename: university-of-amsterdam-info-api-openapi.yml
  format: yaml
  label: University of Amsterdam Info API
  slug: university-of-amsterdam-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-info-api-openapi.yml
- filename: university-of-amsterdam-jobs-api-openapi.yml
  format: yaml
  label: University of Amsterdam Jobs API
  slug: university-of-amsterdam-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-jobs-api-openapi.yml
- filename: university-of-amsterdam-prefixes-api-openapi.yml
  format: yaml
  label: University of Amsterdam Prefixes API
  slug: university-of-amsterdam-prefixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-prefixes-api-openapi.yml
- filename: university-of-amsterdam-queries-api-openapi.yml
  format: yaml
  label: University of Amsterdam Queries API
  slug: university-of-amsterdam-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-queries-api-openapi.yml
- filename: university-of-amsterdam-search-api-openapi.yml
  format: yaml
  label: University of Amsterdam Search API
  slug: university-of-amsterdam-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-search-api-openapi.yml
- filename: university-of-amsterdam-services-api-openapi.yml
  format: yaml
  label: University of Amsterdam Services API
  slug: university-of-amsterdam-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-services-api-openapi.yml
- filename: university-of-amsterdam-sparql-api-openapi.yml
  format: yaml
  label: University of Amsterdam SPARQL API
  slug: university-of-amsterdam-sparql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-sparql-api-openapi.yml
- filename: university-of-amsterdam-stories-api-openapi.yml
  format: yaml
  label: University of Amsterdam Stories API
  slug: university-of-amsterdam-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-stories-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: University Of Amsterdam Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Amsterdam secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of Amsterdam
provider_slug: university-of-amsterdam
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/university-of-amsterdam-lod-triply-api.yaml
  type: http
slug: university-of-amsterdam-authentication
source_filename: university-of-amsterdam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-amsterdam-lod-triply-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/university-of-amsterdam-lod-triply-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/authentication/university-of-amsterdam-authentication.yml
summary_line: http · 1 scheme
tags:
- Education
- Higher Education
- University
- Open Data
- Linked Data
- Library
- Netherlands
- Europe
---
