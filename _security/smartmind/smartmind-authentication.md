---
api_key_in:
- header
api_specs:
- filename: smartmind-thanosql-openapi.json
  format: json
  label: ThanoSQL API
  slug: thanosql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-thanosql-openapi.json
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
