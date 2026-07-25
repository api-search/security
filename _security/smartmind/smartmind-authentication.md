---
api_key_in:
- header
api_specs:
- filename: smartmind-file-api-openapi.yml
  format: yaml
  label: SmartMind file API
  slug: smartmind-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-file-api-openapi.yml
- filename: smartmind-health-api-openapi.yml
  format: yaml
  label: SmartMind health API
  slug: smartmind-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-health-api-openapi.yml
- filename: smartmind-metric-api-openapi.yml
  format: yaml
  label: SmartMind metric API
  slug: smartmind-metric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-metric-api-openapi.yml
- filename: smartmind-query-api-openapi.yml
  format: yaml
  label: SmartMind query API
  slug: smartmind-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-query-api-openapi.yml
- filename: smartmind-schema-api-openapi.yml
  format: yaml
  label: SmartMind schema API
  slug: smartmind-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-schema-api-openapi.yml
- filename: smartmind-table-api-openapi.yml
  format: yaml
  label: SmartMind table API
  slug: smartmind-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-table-api-openapi.yml
- filename: smartmind-table-template-api-openapi.yml
  format: yaml
  label: SmartMind table_template API
  slug: smartmind-table-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-table-template-api-openapi.yml
- filename: smartmind-view-api-openapi.yml
  format: yaml
  label: SmartMind view API
  slug: smartmind-view-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-view-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Smartmind Authentication
name_suffix: Authentication
oauth_flows: []
overview: SmartMind secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SmartMind
provider_slug: smartmind
scheme_count: 1
schemes:
- description: 'Enter: **''Bearer &lt;JWT&gt;''**, where JWT is the access token. Example: Bearer access_token_comes_here'
  in: header
  name: Bearer Auth
  parameter: Authorization
  sources:
  - openapi/smartmind-thanosql-openapi.json
  type: apiKey
slug: smartmind-authentication
source_filename: smartmind-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/smartmind-thanosql-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Enter: **''Bearer &lt;JWT&gt;''**, where JWT is the access token. Example: Bearer\n    access_token_comes_here'\n  sources:\n  - openapi/smartmind-thanosql-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/authentication/smartmind-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Database
- Analytics
- Data
- SQL
- Ontology
- RAG
- Enterprise AI
---
