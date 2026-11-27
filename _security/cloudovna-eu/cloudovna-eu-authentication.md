---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cloudovna-eu-catalog-api-openapi.yml
  format: yaml
  label: Cloudovňa Catalog API
  slug: cloudovna-eu-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-catalog-api-openapi.yml
- filename: cloudovna-eu-health-api-openapi.yml
  format: yaml
  label: Cloudovňa Health API
  slug: cloudovna-eu-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-health-api-openapi.yml
- filename: cloudovna-eu-hooks-api-openapi.yml
  format: yaml
  label: Cloudovňa Hooks API
  slug: cloudovna-eu-hooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-hooks-api-openapi.yml
- filename: cloudovna-eu-images-api-openapi.yml
  format: yaml
  label: Cloudovňa Images API
  slug: cloudovna-eu-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-images-api-openapi.yml
- filename: cloudovna-eu-integrations-api-openapi.yml
  format: yaml
  label: Cloudovňa Integrations API
  slug: cloudovna-eu-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-integrations-api-openapi.yml
- filename: cloudovna-eu-invitations-api-openapi.yml
  format: yaml
  label: Cloudovňa Invitations API
  slug: cloudovna-eu-invitations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-invitations-api-openapi.yml
- filename: cloudovna-eu-invoices-api-openapi.yml
  format: yaml
  label: Cloudovňa Invoices API
  slug: cloudovna-eu-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-invoices-api-openapi.yml
- filename: cloudovna-eu-mcp-api-openapi.yml
  format: yaml
  label: Cloudovňa MCP API
  slug: cloudovna-eu-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-mcp-api-openapi.yml
- filename: cloudovna-eu-oauth-api-openapi.yml
  format: yaml
  label: Cloudovňa OAuth API
  slug: cloudovna-eu-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-oauth-api-openapi.yml
- filename: cloudovna-eu-organizations-api-openapi.yml
  format: yaml
  label: Cloudovňa Organizations API
  slug: cloudovna-eu-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-organizations-api-openapi.yml
- filename: cloudovna-eu-payments-api-openapi.yml
  format: yaml
  label: Cloudovňa Payments API
  slug: cloudovna-eu-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-payments-api-openapi.yml
- filename: cloudovna-eu-pool-api-openapi.yml
  format: yaml
  label: Cloudovňa Pool API
  slug: cloudovna-eu-pool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-pool-api-openapi.yml
- filename: cloudovna-eu-public-api-openapi.yml
  format: yaml
  label: Cloudovňa Public API
  slug: cloudovna-eu-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-public-api-openapi.yml
- filename: cloudovna-eu-services-api-openapi.yml
  format: yaml
  label: Cloudovňa Services API
  slug: cloudovna-eu-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-services-api-openapi.yml
- filename: cloudovna-eu-stacks-api-openapi.yml
  format: yaml
  label: Cloudovňa Stacks API
  slug: cloudovna-eu-stacks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-stacks-api-openapi.yml
- filename: cloudovna-eu-well-known-api-openapi.yml
  format: yaml
  label: Cloudovňa .well Known API
  slug: cloudovna-eu-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudovna-eu/openapi/cloudovna-eu-well-known-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cloudovňa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudovňa declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cloudovňa
provider_slug: cloudovna-eu
scheme_count: 2
schemes:
- applies_to: REST API (https://admin.cloudovna.eu/api) and MCP server (https://admin.cloudovna.eu/mcp)
  description: Personal API token made in the dashboard (Integrations → Cloudovňa API tokens). Starts with cdv_, shown once, expires after 30, 90 or 365 days or never; up to 25 tokens per organization. Access is Read or Manage. Works only in the organization it was made in.
  format: 'Authorization: Bearer cdv_...'
  header: Authorization
  in: header
  name: Bearer
  scheme: bearer
  type: http
- applies_to: MCP server only (https://admin.cloudovna.eu/mcp)
  description: MCP clients sign in with OAuth and choose Manage or Read; access lasts an hour at a time and renews itself while connected. Metadata read with GET from the documented well-known paths (HTTP 200).
  dynamic_client_registration: RFC 7591
  flows:
  - authorization_code
  metadata:
    authorization_server: https://admin.cloudovna.eu/.well-known/oauth-authorization-server
    protected_resource: https://admin.cloudovna.eu/.well-known/oauth-protected-resource/mcp
  name: OAuth (MCP)
  pkce: S256
  scopes:
  - read
  - manage
  type: oauth2
slug: cloudovna-eu-authentication
source_filename: cloudovna-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cloudovna.eu/docs/api.md\ndocs: https://cloudovna.eu/docs/api.md\nrelated_docs:\n- https://cloudovna.eu/docs/mcp.md\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer cdv_...'\n  description: Personal API token made in the dashboard (Integrations → Cloudovňa API tokens). Starts with cdv_, shown once, expires after 30, 90 or 365 days or never; up to 25 tokens per organization. Access is Read or Manage. Works only in the organization it was made in.\n  applies_to: REST API (https://admin.cloudovna.eu/api) and MCP server (https://admin.cloudovna.eu/mcp)\n- name: OAuth (MCP)\n  type: oauth2\n  flows: [authorization_code]\n  pkce: S256\n  dynamic_client_registration: RFC 7591\n  scopes: [read, manage]\n  metadata:\n    authorization_server: https://admin.cloudovna.eu/.well-known/oauth-authorization-server\n    protected_resource: https://admin.cloudovna.eu/.well-known/oauth-protected-resource/mcp\n\
  \  applies_to: MCP server only (https://admin.cloudovna.eu/mcp)\n  description: MCP clients sign in with OAuth and choose Manage or Read; access lasts an hour at a time and renews itself while connected. Metadata read with GET from the documented well-known paths (HTTP 200).\nrestrictions: Tokens cannot sign in/out, change password or email, manage tokens, change billing or pay, link/unlink Docker Hub, GitHub or Cloudflare accounts, or reach staff-only functions.\n"
source_yaml_url: https://artifacts.apis.io/cloudovna-eu/authentication/cloudovna-eu-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cloud Hosting
- Containers
- Docker
- Database
- PostgreSQL
- SQL Server
- European Union
- MCP
---
