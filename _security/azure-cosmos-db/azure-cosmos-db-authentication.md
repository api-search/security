---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: azure-cosmos-db-datatransfer-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Data Transfer API
  slug: azure-cosmos-db-datatransfer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-datatransfer-api-openapi.yml
- filename: azure-cosmos-db-fleets-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Fleets API
  slug: azure-cosmos-db-fleets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-fleets-api-openapi.yml
- filename: azure-cosmos-db-graphapicompute-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Graph API Compute API
  slug: azure-cosmos-db-graphapicompute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-graphapicompute-api-openapi.yml
- filename: azure-cosmos-db-materializedviewsbuilder-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Materialized Views Builder API
  slug: azure-cosmos-db-materializedviewsbuilder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-materializedviewsbuilder-api-openapi.yml
- filename: azure-cosmos-db-notebookworkspacesresource-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Notebook Workspaces Resource API
  slug: azure-cosmos-db-notebookworkspacesresource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-notebookworkspacesresource-api-openapi.yml
- filename: azure-cosmos-db-operations-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Operations API
  slug: azure-cosmos-db-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-operations-api-openapi.yml
- filename: azure-cosmos-db-privatelinkresources-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Private Link Resources API
  slug: azure-cosmos-db-privatelinkresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-privatelinkresources-api-openapi.yml
- filename: azure-cosmos-db-providers-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Providers API
  slug: azure-cosmos-db-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-providers-api-openapi.yml
- filename: azure-cosmos-db-sqldedicatedgateway-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Sql Dedicated Gateway API
  slug: azure-cosmos-db-sqldedicatedgateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-sqldedicatedgateway-api-openapi.yml
- filename: azure-cosmos-db-subscriptions-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Subscriptions API
  slug: azure-cosmos-db-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-subscriptions-api-openapi.yml
- filename: azure-cosmos-db-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Private Endpoint Connections API
  slug: azure-cosmos-db-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-private-endpoint-connections-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Azure Cosmos DB Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- implicit
overview: Azure Cosmos DB secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and implicit flow(s).
provider_name: Azure Cosmos DB
provider_slug: azure-cosmos-db
scheme_count: 3
schemes:
- description: 'Cosmos DB master-key or resource-token HMAC signature. Format:

    `type=master&ver=1.0&sig=<base64-hmac-sha256>` (URL-encoded).

    See https://learn.microsoft.com/en-us/rest/api/cosmos-db/access-control-on-cosmosdb-resources'
  in: header
  name: cosmosAuth
  parameter: Authorization
  sources:
  - openapi/_superseded/azure-cosmos-db-collections-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-databases-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-documents-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-offers-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-permissions-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-stored-procedures-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-triggers-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-user-defined-functions-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-users-api-openapi.yml
  type: apiKey
- description: Microsoft Entra ID OAuth 2.0 bearer token
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: entra
  sources:
  - openapi/_superseded/azure-cosmos-db-collections-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-databases-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-documents-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-offers-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-permissions-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-stored-procedures-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-triggers-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-user-defined-functions-api-openapi.yml
  - openapi/_superseded/azure-cosmos-db-users-api-openapi.yml
  type: oauth2
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-cosmos-db-resource-provider-openapi.yml
  type: oauth2
slug: azure-cosmos-db-authentication
source_filename: azure-cosmos-db-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/azure-cosmos-db-collections-api-openapi.yml, openapi/_superseded/azure-cosmos-db-databases-api-openapi.yml,\n  openapi/_superseded/azure-cosmos-db-documents-api-openapi.yml, openapi/_superseded/azure-cosmos-db-offers-api-openapi.yml,\n  openapi/_superseded/azure-cosmos-db-permissions-api-openapi.yml, openapi/azure-cosmos-db-resource-provider-openapi.yml,\n  openapi/_superseded/azure-cosmos-db-stored-procedures-api-openapi.yml, openapi/_superseded/azure-cosmos-db-triggers-api-openapi.yml,\n  openapi/_superseded/azure-cosmos-db-user-defined-functions-api-openapi.yml, openapi/_superseded/azure-cosmos-db-users-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  - implicit\nschemes:\n- name: cosmosAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Cosmos DB master-key or resource-token HMAC signature.\
  \ Format:\n    `type=master&ver=1.0&sig=<base64-hmac-sha256>` (URL-encoded).\n    See https://learn.microsoft.com/en-us/rest/api/cosmos-db/access-control-on-cosmosdb-resources\n  sources:\n  - openapi/_superseded/azure-cosmos-db-collections-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-databases-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-documents-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-offers-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-permissions-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-stored-procedures-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-triggers-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-user-defined-functions-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-users-api-openapi.yml\n- name: entra\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID\
  \ OAuth 2.0 bearer token\n  sources:\n  - openapi/_superseded/azure-cosmos-db-collections-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-databases-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-documents-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-offers-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-permissions-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-stored-procedures-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-triggers-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-user-defined-functions-api-openapi.yml\n  - openapi/_superseded/azure-cosmos-db-users-api-openapi.yml\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/azure-cosmos-db-resource-provider-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/azure-cosmos-db/authentication/azure-cosmos-db-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Database
- NoSQL
- Document Database
- Vector Search
- Globally Distributed
- Cloud
- Microsoft Azure
---
