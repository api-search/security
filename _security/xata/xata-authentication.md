---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Xata Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://api.xata.tech/openapi.json
- filename: openapi.json
  format: json
  label: Xata SQL Gateway
  slug: sql-gateway
  spec_type: OpenAPI
  url: https://api.xata.tech/openapi.json
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Xata Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Xata secures its APIs with apiKey, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Xata
provider_slug: xata
scheme_count: 4
schemes:
- name: oidc
  openIdConnectUrl: https://auth.xata.io/realms/xata/.well-known/openid-configuration
  sources:
  - openapi/xata-management-api-openapi.yml
  type: openIdConnect
- description: 'API key authentication using Bearer token format: Bearer <api_key>'
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/xata-management-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://auth.xata.io/realms/xata/protocol/openid-connect/auth
    flow: implicit
    scopes: 13
  name: xata
  sources:
  - openapi/xata-management-api-openapi.yml
  type: oauth2
- description: Branch PostgreSQL connection string (`postgres://user:pass@{branch}.{region}.xata.tech/db`), including the embedded password. The hostname selects the target branch, region, and endpoint type (the `-rw`/`-ro` suffix, see `EndpointType`), and must match the request host. Obtain it from the Xata dashboard or the control-plane API. This is the only credential the gateway accepts; the control-plane AP
  in: header
  name: branchConnectionString
  parameter: Connection-String
  sources:
  - openapi/xata-management-api-openapi.yml
  type: apiKey
slug: xata-authentication
source_filename: xata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xata-management-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - implicit\nschemes:\n- name: oidc\n  type: openIdConnect\n  openIdConnectUrl: https://auth.xata.io/realms/xata/.well-known/openid-configuration\n  sources:\n  - openapi/xata-management-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key authentication using Bearer token format: Bearer <api_key>'\n  sources:\n  - openapi/xata-management-api-openapi.yml\n- name: xata\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://auth.xata.io/realms/xata/protocol/openid-connect/auth\n    scopes: 13\n  sources:\n  - openapi/xata-management-api-openapi.yml\n- name: branchConnectionString\n  type: apiKey\n  in: header\n  parameter: Connection-String\n  description: Branch PostgreSQL connection string (`postgres://user:pass@{branch}.{region}.xata.tech/db`),\n\
  \    including the embedded password. The hostname selects the target branch, region, and endpoint\n    type (the `-rw`/`-ro` suffix, see `EndpointType`), and must match the request host. Obtain\n    it from the Xata dashboard or the control-plane API. This is the only credential the gateway\n    accepts; the control-plane AP\n  sources:\n  - openapi/xata-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xata/refs/heads/main/authentication/xata-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 4 schemes
tags:
- Database
- Postgres
- Serverless
- Developer Tools
- Branching
- AI Agent
---
