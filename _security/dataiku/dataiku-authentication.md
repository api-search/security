---
api_key_in:
- header
api_specs:
- filename: index.html
  format: yaml
  label: Dataiku Public API
  slug: dataiku-public-api
  spec_type: OpenAPI
  url: https://doc.dataiku.com/dss/latest/publicapi/rest/index.html
- filename: dataiku-api-node-admin-openapi.yml
  format: yaml
  label: Dataiku API Node Administration API
  slug: dataiku-api-node-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataiku/refs/heads/main/openapi/dataiku-api-node-admin-openapi.yml
- filename: dataiku-govern-api-openapi.yml
  format: yaml
  label: Dataiku Govern API
  slug: dataiku-govern-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataiku/refs/heads/main/openapi/dataiku-govern-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dataiku Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dataiku secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dataiku
provider_slug: dataiku
scheme_count: 1
schemes:
- description: Admin API key passed as Bearer token
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/dataiku-api-node-admin-openapi.yml
  - openapi/dataiku-govern-api-openapi.yml
  - openapi/dataiku-public-api-openapi.yml
  type: apiKey
slug: dataiku-authentication
source_filename: dataiku-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dataiku-api-node-admin-openapi.yml, openapi/dataiku-govern-api-openapi.yml,\n  openapi/dataiku-public-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Admin API key passed as Bearer token\n  sources:\n  - openapi/dataiku-api-node-admin-openapi.yml\n  - openapi/dataiku-govern-api-openapi.yml\n  - openapi/dataiku-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dataiku/refs/heads/main/authentication/dataiku-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Artificial Intelligence
- Data Platform
- Data Science
- Machine Learning
---
