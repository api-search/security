---
api_key_in: []
api_specs:
- filename: azure-databricks-openapi.yml
  format: yaml
  label: Azure Databricks REST API
  slug: azure-databricks-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/openapi/azure-databricks-openapi.yml
- filename: azure-databricks-openapi.yml
  format: yaml
  label: Clusters API
  slug: clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/openapi/azure-databricks-openapi.yml
- filename: azure-databricks-openapi.yml
  format: yaml
  label: Jobs API
  slug: jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/openapi/azure-databricks-openapi.yml
- filename: azure-databricks-openapi.yml
  format: yaml
  label: Workspace API
  slug: workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/openapi/azure-databricks-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Databricks Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Azure Databricks secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Azure Databricks
provider_slug: azure-databricks
scheme_count: 2
schemes:
- description: Databricks personal access token. Pass the token in the Authorization header as Bearer <token>.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/azure-databricks-openapi.yml
  type: http
- description: Azure Active Directory token for authenticating with Azure Databricks. Supports both user and service principal authentication.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token
  name: AzureADToken
  sources:
  - openapi/azure-databricks-openapi.yml
  type: oauth2
slug: azure-databricks-authentication
source_filename: azure-databricks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-databricks-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Databricks personal access token. Pass the token in the Authorization header\n    as Bearer <token>.\n  sources:\n  - openapi/azure-databricks-openapi.yml\n- name: AzureADToken\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/{tenant_id}/oauth2/v2.0/token\n    scopes: 1\n  description: Azure Active Directory token for authenticating with Azure Databricks. Supports\n    both user and service principal authentication.\n  sources:\n  - openapi/azure-databricks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-databricks/refs/heads/main/authentication/azure-databricks-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Analytics
- Apache Spark
- Big Data
- Data Engineering
- Machine Learning
---
