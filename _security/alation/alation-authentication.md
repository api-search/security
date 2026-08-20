---
api_key_in: []
api_specs:
- filename: alation-aggregated-context-api-openapi.yml
  format: yaml
  label: Alation Aggregated Context API
  slug: alation-aggregated-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-aggregated-context-api-openapi.yml
- filename: alation-columns-api-openapi.yml
  format: yaml
  label: Alation Columns API
  slug: alation-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-columns-api-openapi.yml
- filename: alation-custom-fields-api-openapi.yml
  format: yaml
  label: Alation Custom Fields API
  slug: alation-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-custom-fields-api-openapi.yml
- filename: alation-data-quality-api-openapi.yml
  format: yaml
  label: Alation Data Quality API
  slug: alation-data-quality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-data-quality-api-openapi.yml
- filename: alation-data-sources-api-openapi.yml
  format: yaml
  label: Alation Data Sources API
  slug: alation-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-data-sources-api-openapi.yml
- filename: alation-dataflows-api-openapi.yml
  format: yaml
  label: Alation Dataflows API
  slug: alation-dataflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-dataflows-api-openapi.yml
- filename: alation-glossary-terms-api-openapi.yml
  format: yaml
  label: Alation Glossary Terms API
  slug: alation-glossary-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-glossary-terms-api-openapi.yml
- filename: alation-lineage-api-openapi.yml
  format: yaml
  label: Alation Lineage API
  slug: alation-lineage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-lineage-api-openapi.yml
- filename: alation-policies-api-openapi.yml
  format: yaml
  label: Alation Policies API
  slug: alation-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-policies-api-openapi.yml
- filename: alation-schemas-api-openapi.yml
  format: yaml
  label: Alation Schemas API
  slug: alation-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-schemas-api-openapi.yml
- filename: alation-search-api-openapi.yml
  format: yaml
  label: Alation Search API
  slug: alation-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-search-api-openapi.yml
- filename: alation-tables-api-openapi.yml
  format: yaml
  label: Alation Tables API
  slug: alation-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alation/refs/heads/main/openapi/alation-tables-api-openapi.yml
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
- Artificial Intelligence
---
