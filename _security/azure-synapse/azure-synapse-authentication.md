---
api_key_in: []
api_specs:
- filename: synapse.json
  format: json
  label: Azure Synapse REST API
  slug: azure-synapse-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/synapse/resource-manager/Microsoft.Synapse/stable/2021-06-01/synapse.json
- filename: azure-synapse-openapi.yaml
  format: yaml
  label: Azure Synapse Pipeline API
  slug: azure-synapse-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-synapse/refs/heads/main/openapi/azure-synapse-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Synapse Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Synapse Analytics secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Synapse Analytics
provider_slug: azure-synapse
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-synapse-openapi.yaml
  type: oauth2
slug: azure-synapse-authentication
source_filename: azure-synapse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-synapse-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  sources:\n  - openapi/azure-synapse-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-synapse/refs/heads/main/authentication/azure-synapse-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Apache Spark
- Big Data
- Data Warehouse
- ETL
- SQL
---
