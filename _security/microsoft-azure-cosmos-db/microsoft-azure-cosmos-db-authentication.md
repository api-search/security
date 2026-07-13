---
api_key_in:
- header
api_specs:
- filename: microsoft-azure-cosmos-db-openapi.yml
  format: yaml
  label: Azure Cosmos DB API
  slug: azure-cosmos-db-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cosmos-db/refs/heads/main/openapi/microsoft-azure-cosmos-db-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Cosmos Db Authentication
name_suffix: Authentication
oauth_flows: []
overview: microsoft-azure-cosmos-db secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: microsoft-azure-cosmos-db
provider_slug: microsoft-azure-cosmos-db
scheme_count: 1
schemes:
- description: Master key or resource token in Authorization header
  in: header
  name: masterKey
  parameter: Authorization
  sources:
  - openapi/microsoft-azure-cosmos-db-openapi.yml
  type: apiKey
slug: microsoft-azure-cosmos-db-authentication
source_filename: microsoft-azure-cosmos-db-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-cosmos-db-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: masterKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Master key or resource token in Authorization header\n  sources:\n  - openapi/microsoft-azure-cosmos-db-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-cosmos-db/refs/heads/main/authentication/microsoft-azure-cosmos-db-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
