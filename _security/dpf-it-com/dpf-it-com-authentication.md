---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dpf-it-com-account-api-openapi.yml
  format: yaml
  label: DPF Account API
  slug: dpf-it-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-account-api-openapi.yml
- filename: dpf-it-com-authentication-api-openapi.yml
  format: yaml
  label: DPF Authentication API
  slug: dpf-it-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-authentication-api-openapi.yml
- filename: dpf-it-com-connections-api-openapi.yml
  format: yaml
  label: DPF Connections API
  slug: dpf-it-com-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-connections-api-openapi.yml
- filename: dpf-it-com-contact-api-openapi.yml
  format: yaml
  label: DPF Contact API
  slug: dpf-it-com-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-contact-api-openapi.yml
- filename: dpf-it-com-data-specs-api-openapi.yml
  format: yaml
  label: DPF Data Specs API
  slug: dpf-it-com-data-specs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-data-specs-api-openapi.yml
- filename: dpf-it-com-iceberg-rest-catalog-api-openapi.yml
  format: yaml
  label: DPF Iceberg REST Catalog API
  slug: dpf-it-com-iceberg-rest-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-iceberg-rest-catalog-api-openapi.yml
- filename: dpf-it-com-job-triggers-api-openapi.yml
  format: yaml
  label: DPF Job Triggers API
  slug: dpf-it-com-job-triggers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-job-triggers-api-openapi.yml
- filename: dpf-it-com-mcp-api-openapi.yml
  format: yaml
  label: DPF MCP API
  slug: dpf-it-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-mcp-api-openapi.yml
- filename: dpf-it-com-oauth-2-1-authorization-server-api-openapi.yml
  format: yaml
  label: DPF OAuth 2.1 Authorization Server API
  slug: dpf-it-com-oauth-2-1-authorization-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-oauth-2-1-authorization-server-api-openapi.yml
- filename: dpf-it-com-query-api-openapi.yml
  format: yaml
  label: DPF Query API
  slug: dpf-it-com-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-query-api-openapi.yml
- filename: dpf-it-com-workspaces-api-openapi.yml
  format: yaml
  label: DPF Workspaces API
  slug: dpf-it-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dpf-it-com/openapi/dpf-it-com-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: DPF Authentication
name_suffix: Authentication
oauth_flows: []
overview: DPF secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DPF
provider_slug: dpf-it-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token obtained from login or registration
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/dpf-it-com-openapi.yml
  type: http
slug: dpf-it-com-authentication
source_filename: dpf-it-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/dpf-it-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained from login or registration\n  sources:\n  - openapi/dpf-it-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/dpf-it-com/authentication/dpf-it-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Data
- Artificial Intelligence
- ETL
- Apache Iceberg
- Platform
- Company
---
