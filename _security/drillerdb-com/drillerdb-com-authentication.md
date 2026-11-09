---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: drillerdb-com-conferences-api-openapi.yml
  format: yaml
  label: DrillerDB Conferences API
  slug: drillerdb-com-conferences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-conferences-api-openapi.yml
- filename: drillerdb-com-contacts-api-openapi.yml
  format: yaml
  label: DrillerDB Contacts API
  slug: drillerdb-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-contacts-api-openapi.yml
- filename: drillerdb-com-documentation-api-openapi.yml
  format: yaml
  label: DrillerDB Documentation API
  slug: drillerdb-com-documentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-documentation-api-openapi.yml
- filename: drillerdb-com-driller-directory-api-openapi.yml
  format: yaml
  label: DrillerDB Driller directory API
  slug: drillerdb-com-driller-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-driller-directory-api-openapi.yml
- filename: drillerdb-com-enterprise-mcp-api-openapi.yml
  format: yaml
  label: DrillerDB Enterprise MCP API
  slug: drillerdb-com-enterprise-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-enterprise-mcp-api-openapi.yml
- filename: drillerdb-com-equipment-api-openapi.yml
  format: yaml
  label: DrillerDB Equipment API
  slug: drillerdb-com-equipment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-equipment-api-openapi.yml
- filename: drillerdb-com-geocoding-api-openapi.yml
  format: yaml
  label: DrillerDB Geocoding API
  slug: drillerdb-com-geocoding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-geocoding-api-openapi.yml
- filename: drillerdb-com-inventory-api-openapi.yml
  format: yaml
  label: DrillerDB Inventory API
  slug: drillerdb-com-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-inventory-api-openapi.yml
- filename: drillerdb-com-invoices-api-openapi.yml
  format: yaml
  label: DrillerDB Invoices API
  slug: drillerdb-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-invoices-api-openapi.yml
- filename: drillerdb-com-platform-api-openapi.yml
  format: yaml
  label: DrillerDB Platform API
  slug: drillerdb-com-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-platform-api-openapi.yml
- filename: drillerdb-com-projects-api-openapi.yml
  format: yaml
  label: DrillerDB Projects API
  slug: drillerdb-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-projects-api-openapi.yml
- filename: drillerdb-com-well-data-api-openapi.yml
  format: yaml
  label: DrillerDB Well data API
  slug: drillerdb-com-well-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-well-data-api-openapi.yml
- filename: drillerdb-com-work-orders-api-openapi.yml
  format: yaml
  label: DrillerDB Work Orders API
  slug: drillerdb-com-work-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drillerdb-com/openapi/drillerdb-com-work-orders-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Drillerdb Com Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: DrillerDB secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: DrillerDB
provider_slug: drillerdb-com
scheme_count: 2
schemes:
- description: Company API key issued in DrillerDB Settings > API Access (Enterprise plan). Keys are scoped; the scopes a key may hold are projects:read, invoices:read, work_orders:read, contacts:read, equipment:read and inventory:read. A key lacking the scope an operation needs receives 403 INSUFFICIENT_SCOPE with meta.required_scope.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/drillerdb-com-openapi.json
  type: apiKey
- description: 'OAuth 2.1 authorization-code flow with PKCE (S256), as published at https://enterprise.drillerdb.com/.well-known/oauth-authorization-server. Dynamic client registration is available at https://enterprise.drillerdb.com/oauth/register. Tokens are presented as Bearer in the Authorization header. Protected-resource metadata (RFC 9728): https://enterprise.drillerdb.com/.well-known/oauth-protected-resou'
  flows:
  - authorizationUrl: https://enterprise.drillerdb.com/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://enterprise.drillerdb.com/oauth/token
  name: EnterpriseMcpOAuth
  sources:
  - openapi/drillerdb-com-openapi.json
  type: oauth2
slug: drillerdb-com-authentication
source_filename: drillerdb-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/drillerdb-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Company API key issued in DrillerDB Settings > API Access (Enterprise plan).\n    Keys are scoped; the scopes a key may hold are projects:read, invoices:read, work_orders:read,\n    contacts:read, equipment:read and inventory:read. A key lacking the scope an operation needs\n    receives 403 INSUFFICIENT_SCOPE with meta.required_scope.\n  sources:\n  - openapi/drillerdb-com-openapi.json\n- name: EnterpriseMcpOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://enterprise.drillerdb.com/oauth/authorize\n    tokenUrl: https://enterprise.drillerdb.com/oauth/token\n    scopes: 1\n  description: 'OAuth 2.1 authorization-code flow with PKCE (S256), as\
  \ published at https://enterprise.drillerdb.com/.well-known/oauth-authorization-server.\n    Dynamic client registration is available at https://enterprise.drillerdb.com/oauth/register.\n    Tokens are presented as Bearer in the Authorization header. Protected-resource metadata\n    (RFC 9728): https://enterprise.drillerdb.com/.well-known/oauth-protected-resou'\n  sources:\n  - openapi/drillerdb-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/drillerdb-com/authentication/drillerdb-com-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Water Well
- DrillingSoftware
- PumpService
- Project Management
- Software-as-a-Service
---
