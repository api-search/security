---
api_key_in: []
api_specs:
- filename: power-query-fabric-dataflow-swagger.json
  format: json
  label: Fabric Dataflow REST API (Power Query)
  slug: fabric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/power-query/refs/heads/main/openapi/power-query-fabric-dataflow-swagger.json
auth_types: []
description: The Power Query programmatic surface (the Fabric Dataflow REST API on api.fabric.microsoft.com) authenticates exclusively with Microsoft Entra ID OAuth 2.0 bearer tokens. There are no API keys and no basic auth. The published Swagger carries no securityDefinitions block — the auth model is documented on the Fabric REST articles rather than in the contract, which is recorded here as a contract gap, not as an absence of authentication.
kind: authentication
layout: security
method: searched
name: Power Query Authentication
name_suffix: Authentication
oauth_flows: []
overview: Power Query declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Power Query
provider_slug: power-query
scheme_count: 1
schemes:
- authorization_endpoint: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
  discovery: https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration
  discovery_status: 200
  flows:
  - authorization_code
  - client_credentials
  - device_code
  format: Bearer <access_token>
  header: Authorization
  id: entra-oauth2
  in: header
  issuer: https://login.microsoftonline.com/{tenantid}/v2.0
  name: Microsoft Entra ID (OAuth 2.0 / OpenID Connect)
  resource: https://api.fabric.microsoft.com
  scopes_reference: scopes/power-query-scopes.yml
  token_endpoint: https://login.microsoftonline.com/common/oauth2/v2.0/token
  type: oauth2
slug: power-query-authentication
source_filename: power-query-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://learn.microsoft.com/en-us/rest/api/fabric/articles/identity-support and\n  https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration\ndocs: https://learn.microsoft.com/en-us/rest/api/fabric/articles/scopes\nprovider: Power Query\nproviderId: power-query\ndescription: >-\n  The Power Query programmatic surface (the Fabric Dataflow REST API on\n  api.fabric.microsoft.com) authenticates exclusively with Microsoft Entra ID\n  OAuth 2.0 bearer tokens. There are no API keys and no basic auth. The published\n  Swagger carries no securityDefinitions block — the auth model is documented on\n  the Fabric REST articles rather than in the contract, which is recorded here as\n  a contract gap, not as an absence of authentication.\nprimary_style: oauth2\nschemes:\n  - id: entra-oauth2\n    type: oauth2\n    name: Microsoft Entra ID (OAuth 2.0 / OpenID Connect)\n    in: header\n    header: Authorization\n\
  \    format: 'Bearer <access_token>'\n    flows:\n      - authorization_code\n      - client_credentials\n      - device_code\n    authorization_endpoint: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    token_endpoint: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    issuer: https://login.microsoftonline.com/{tenantid}/v2.0\n    discovery: https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration\n    discovery_status: 200\n    resource: https://api.fabric.microsoft.com\n    scopes_reference: scopes/power-query-scopes.yml\nidentities_supported:\n  - identity: user\n    supported: true\n  - identity: service principal\n    supported: true\n  - identity: managed identity\n    supported: true\n    note: >-\n      Per the Fabric scopes article, direct access by service principals and\n      managed identities is governed by Fabric admin tenant switches and\n      workspace permissions rather than by delegated scopes.\nauthorization_model:\n\
  \  - layer: Entra delegated scope\n    note: Applies only to delegated (on-behalf-of-user) access.\n  - layer: Fabric workspace role\n    note: >-\n      Every Dataflow operation additionally requires a workspace role. Creating a\n      dataflow requires the contributor workspace role; reading a definition\n      requires read permission; delete requires write permission.\n  - layer: Fabric tenant admin switches\n    note: >-\n      Tenant admins can disable service-principal API access and features such as\n      soft delete independently of any token the caller holds.\ncontract_gaps:\n  - >-\n    openapi/power-query-fabric-dataflow-swagger.json declares `\"security\": []`\n    and no `securityDefinitions`. A client generated straight from the spec would\n    emit unauthenticated calls. Auth is documented only in prose on the operation\n    descriptions and the Fabric REST articles.\nevidence:\n  - url: https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration\n \
  \   status: 200\n  - url: https://learn.microsoft.com/en-us/rest/api/fabric/articles/scopes\n    status: 200\n  - url: https://learn.microsoft.com/en-us/rest/api/fabric/dataflow/items/create-dataflow\n    status: 200\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n    url: https://apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power-query/refs/heads/main/authentication/power-query-authentication.yml
summary_line: 1 scheme
tags:
- Business Intelligence
- Data Integration
- Data Transformation
- ETL
- Microsoft
- Microsoft Fabric
- Power BI
- Dataflows
- M Language
- Data Connectors
- Self-Service ETL
---
