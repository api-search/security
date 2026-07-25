---
api_key_in:
- header
api_specs:
- filename: azure-cosmos-db-collections-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Collections API
  slug: azure-cosmos-db-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-cosmos-db/refs/heads/main/openapi/azure-cosmos-db-collections-api-openapi.yml
- filename: azure-cosmos-db-databases-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Databases API
  slug: azure-cosmos-db-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-cosmos-db/refs/heads/main/openapi/azure-cosmos-db-databases-api-openapi.yml
- filename: azure-cosmos-db-documents-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Documents API
  slug: azure-cosmos-db-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-cosmos-db/refs/heads/main/openapi/azure-cosmos-db-documents-api-openapi.yml
- filename: azure-cosmos-db-offers-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Offers API
  slug: azure-cosmos-db-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-cosmos-db/refs/heads/main/openapi/azure-cosmos-db-offers-api-openapi.yml
- filename: azure-cosmos-db-permissions-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Permissions API
  slug: azure-cosmos-db-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-cosmos-db/refs/heads/main/openapi/azure-cosmos-db-permissions-api-openapi.yml
- filename: azure-cosmos-db-stored-procedures-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Stored Procedures API
  slug: azure-cosmos-db-stored-procedures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-cosmos-db/refs/heads/main/openapi/azure-cosmos-db-stored-procedures-api-openapi.yml
- filename: azure-cosmos-db-triggers-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Triggers API
  slug: azure-cosmos-db-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-cosmos-db/refs/heads/main/openapi/azure-cosmos-db-triggers-api-openapi.yml
- filename: azure-cosmos-db-user-defined-functions-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB User Defined Functions API
  slug: azure-cosmos-db-user-defined-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-cosmos-db/refs/heads/main/openapi/azure-cosmos-db-user-defined-functions-api-openapi.yml
- filename: azure-cosmos-db-users-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Users API
  slug: azure-cosmos-db-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-cosmos-db/refs/heads/main/openapi/azure-cosmos-db-users-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Cosmos Db Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Azure Cosmos DB secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Azure Cosmos DB
provider_slug: azure-cosmos-db
scheme_count: 2
schemes:
- description: 'Cosmos DB master-key or resource-token HMAC signature. Format:

    `type=master&ver=1.0&sig=<base64-hmac-sha256>` (URL-encoded).

    See https://learn.microsoft.com/en-us/rest/api/cosmos-db/access-control-on-cosmosdb-resources'
  in: header
  name: cosmosAuth
  parameter: Authorization
  sources:
  - openapi/azure-cosmos-db-openapi.yml
  type: apiKey
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  sources:
  - openapi/azure-cosmos-db-openapi.yml
  type: oauth2
slug: azure-cosmos-db-authentication
source_filename: azure-cosmos-db-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-cosmos-db-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: cosmosAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Cosmos DB master-key or resource-token HMAC signature. Format:\n    `type=master&ver=1.0&sig=<base64-hmac-sha256>` (URL-encoded).\n    See https://learn.microsoft.com/en-us/rest/api/cosmos-db/access-control-on-cosmosdb-resources\n  sources:\n  - openapi/azure-cosmos-db-openapi.yml\n- name: entra\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0 bearer token\n  sources:\n  - openapi/azure-cosmos-db-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-cosmos-db/refs/heads/main/authentication/azure-cosmos-db-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Database
- NoSQL
- Document Database
- Vector Database
- Globally Distributed
- Cloud
- Azure
---
