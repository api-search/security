---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datafiniti-properties-api-openapi.yml
  format: yaml
  label: Datafiniti Property Data API
  slug: property-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-properties-api-openapi.yml
- filename: datafiniti-people-api-openapi.yml
  format: yaml
  label: Datafiniti People Data API
  slug: people-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-people-api-openapi.yml
- filename: datafiniti-businesses-api-openapi.yml
  format: yaml
  label: Datafiniti Business Data API
  slug: business-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-businesses-api-openapi.yml
- filename: datafiniti-products-api-openapi.yml
  format: yaml
  label: Datafiniti Product Data API
  slug: product-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-products-api-openapi.yml
- filename: datafiniti-downloads-api-openapi.yml
  format: yaml
  label: Datafiniti Downloads API
  slug: downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-downloads-api-openapi.yml
- filename: datafiniti-views-api-openapi.yml
  format: yaml
  label: Datafiniti Views API
  slug: views-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-views-api-openapi.yml
- filename: datafiniti-real-time-data-requests-api-openapi.yml
  format: yaml
  label: Datafiniti Real-time Data Requests API
  slug: real-time-data-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-real-time-data-requests-api-openapi.yml
- filename: datafiniti-authentication-api-openapi.yml
  format: yaml
  label: Datafiniti Authentication API
  slug: datafiniti-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-authentication-api-openapi.yml
- filename: datafiniti-account-api-openapi.yml
  format: yaml
  label: Datafiniti Account API
  slug: account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-account-api-openapi.yml
- filename: datafiniti-status-api-openapi.yml
  format: yaml
  label: Datafiniti Status API
  slug: status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datafiniti/openapi/datafiniti-status-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Datafiniti Authentication
name_suffix: Authentication
oauth_flows: []
overview: Datafiniti declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Datafiniti
provider_slug: datafiniti
scheme_count: 2
schemes:
- applies_to: REST API v4 and MCP server
  header: Authorization
  in: header
  name: bearerAuth
  obtain:
  - POST https://api.datafiniti.co/v4/auth
  - https://portal.datafiniti.co/settings/api
  - Postman collection download
  scheme: bearer
  type: http
- applies_to: MCP server from claude.ai
  authorization_endpoint: https://api.datafiniti.co/authorize
  evidence: https://api.datafiniti.co/.well-known/oauth-authorization-server
  flows:
  - authorization_code (PKCE S256)
  - refresh_token
  name: mcpOAuth
  scopes:
  - offline_access
  token_endpoint: https://api.datafiniti.co/token
  type: oauth2
slug: datafiniti-authentication
source_filename: datafiniti-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: searched\nsource: https://docs.datafiniti.co/reference/authentication.md\ndocs: https://docs.datafiniti.co/reference/authentication\nsummary:\n  primary: bearer\n  note: POST /auth exchanges account email + password for a bearer token. The same token is available without sending\n    a password from the portal API settings page and the downloadable Postman collection (https://docs.datafiniti.co/docs/get-your-postman-collection-and-token).\n    It regenerates when the account password changes. Datafiniti publishes no token TTL.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  obtain:\n  - POST https://api.datafiniti.co/v4/auth\n  - https://portal.datafiniti.co/settings/api\n  - Postman collection download\n  applies_to: REST API v4 and MCP server\n- name: mcpOAuth\n  type: oauth2\n  flows:\n  - authorization_code (PKCE S256)\n  - refresh_token\n  authorization_endpoint: https://api.datafiniti.co/authorize\n\
  \  token_endpoint: https://api.datafiniti.co/token\n  scopes:\n  - offline_access\n  applies_to: MCP server from claude.ai\n  evidence: https://api.datafiniti.co/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/datafiniti/authentication/datafiniti-authentication.yml
summary_line: 2 schemes
tags:
- Business Data
- Data Aggregation
- Data as a Service
- Data Enrichment
- MCP
- People Data
- Product Data
- Property Data
- Real Estate
---
