---
api_key_in: []
api_specs:
- filename: dremio-intelligent-lakehouse-platform-authentication-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Authentication API
  slug: dremio-intelligent-lakehouse-platform-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-authentication-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-catalog-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Catalog API
  slug: dremio-intelligent-lakehouse-platform-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-catalog-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-jobs-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Jobs API
  slug: dremio-intelligent-lakehouse-platform-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-jobs-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-pat-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform PAT API
  slug: dremio-intelligent-lakehouse-platform-pat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-pat-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-reflections-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Reflections API
  slug: dremio-intelligent-lakehouse-platform-reflections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-reflections-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-roles-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Roles API
  slug: dremio-intelligent-lakehouse-platform-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-roles-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-scripts-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Scripts API
  slug: dremio-intelligent-lakehouse-platform-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-scripts-api-openapi.yml
- filename: dremio-intelligent-lakehouse-platform-sources-api-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform Sources API
  slug: dremio-intelligent-lakehouse-platform-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-sources-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dremio Intelligent Lakehouse Platform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dremio | Intelligent Lakehouse Platform secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dremio | Intelligent Lakehouse Platform
provider_slug: dremio-intelligent-lakehouse-platform
scheme_count: 1
schemes:
- description: OAuth access token or Personal Access Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dremio-intelligent-lakehouse-platform-openapi.yml
  type: http
slug: dremio-intelligent-lakehouse-platform-authentication
source_filename: dremio-intelligent-lakehouse-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dremio-intelligent-lakehouse-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth access token or Personal Access Token\n  sources:\n  - openapi/dremio-intelligent-lakehouse-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/authentication/dremio-intelligent-lakehouse-platform-authentication.yml
summary_line: http · 1 scheme
tags:
- Data
- Analytics
- Lakehouse
- Apache Iceberg
- SQL
- Artificial Intelligence
---
