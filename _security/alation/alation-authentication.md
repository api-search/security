---
api_key_in: []
api_specs:
- filename: alation-data-catalog-openapi.yaml
  format: yaml
  label: Alation Data Catalog API
  slug: data-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-data-catalog-openapi.yaml
- filename: alation-lineage-openapi.yaml
  format: yaml
  label: Alation Lineage API
  slug: lineage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-lineage-openapi.yaml
- filename: alation-governance-openapi.yaml
  format: yaml
  label: Alation Governance API
  slug: governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-governance-openapi.yaml
- filename: alation-search-openapi.yaml
  format: yaml
  label: Alation Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-search-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Alation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alation secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Alation
provider_slug: alation
scheme_count: 1
schemes:
- description: API access token obtained from /integration/v1/createRefreshToken/
  name: BearerToken
  scheme: bearer
  sources:
  - openapi/alation-data-catalog-openapi.yaml
  - openapi/alation-governance-openapi.yaml
  - openapi/alation-lineage-openapi.yaml
  - openapi/alation-search-openapi.yaml
  type: http
slug: alation-authentication
source_filename: alation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alation-data-catalog-openapi.yaml, openapi/alation-governance-openapi.yaml,\n  openapi/alation-lineage-openapi.yaml, openapi/alation-search-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: API access token obtained from /integration/v1/createRefreshToken/\n  sources:\n  - openapi/alation-data-catalog-openapi.yaml\n  - openapi/alation-governance-openapi.yaml\n  - openapi/alation-lineage-openapi.yaml\n  - openapi/alation-search-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/authentication/alation-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Catalog
- Data Governance
- Data Intelligence
- Data Lineage
- Data Quality
- Business Glossary
- Metadata Management
- AI
---
