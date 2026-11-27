---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cloudpepper-io-backup-providers-api-openapi.yml
  format: yaml
  label: Cloudpepper Backup Providers API
  slug: cloudpepper-io-backup-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudpepper-io/openapi/cloudpepper-io-backup-providers-api-openapi.yml
- filename: cloudpepper-io-backup-schedules-api-openapi.yml
  format: yaml
  label: Cloudpepper Backup Schedules API
  slug: cloudpepper-io-backup-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudpepper-io/openapi/cloudpepper-io-backup-schedules-api-openapi.yml
- filename: cloudpepper-io-backups-api-openapi.yml
  format: yaml
  label: Cloudpepper Backups API
  slug: cloudpepper-io-backups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudpepper-io/openapi/cloudpepper-io-backups-api-openapi.yml
- filename: cloudpepper-io-billing-api-openapi.yml
  format: yaml
  label: Cloudpepper Billing API
  slug: cloudpepper-io-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudpepper-io/openapi/cloudpepper-io-billing-api-openapi.yml
- filename: cloudpepper-io-instance-logs-api-openapi.yml
  format: yaml
  label: Cloudpepper Instance Logs API
  slug: cloudpepper-io-instance-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudpepper-io/openapi/cloudpepper-io-instance-logs-api-openapi.yml
- filename: cloudpepper-io-instance-modules-api-openapi.yml
  format: yaml
  label: Cloudpepper Instance Modules API
  slug: cloudpepper-io-instance-modules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudpepper-io/openapi/cloudpepper-io-instance-modules-api-openapi.yml
- filename: cloudpepper-io-instance-templates-api-openapi.yml
  format: yaml
  label: Cloudpepper Instance Templates API
  slug: cloudpepper-io-instance-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudpepper-io/openapi/cloudpepper-io-instance-templates-api-openapi.yml
- filename: cloudpepper-io-odoo-instances-api-openapi.yml
  format: yaml
  label: Cloudpepper Odoo Instances API
  slug: cloudpepper-io-odoo-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudpepper-io/openapi/cloudpepper-io-odoo-instances-api-openapi.yml
- filename: cloudpepper-io-query-insights-api-openapi.yml
  format: yaml
  label: Cloudpepper Query Insights API
  slug: cloudpepper-io-query-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudpepper-io/openapi/cloudpepper-io-query-insights-api-openapi.yml
- filename: cloudpepper-io-server-info-api-openapi.yml
  format: yaml
  label: Cloudpepper Server Info API
  slug: cloudpepper-io-server-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudpepper-io/openapi/cloudpepper-io-server-info-api-openapi.yml
- filename: cloudpepper-io-users-api-openapi.yml
  format: yaml
  label: Cloudpepper Users API
  slug: cloudpepper-io-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cloudpepper-io/openapi/cloudpepper-io-users-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cloudpepper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudpepper secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cloudpepper
provider_slug: cloudpepper-io
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'Bearer token on every REST endpoint. Cloudpepper API keys (prefix "aak-") are an Agency feature, created in the dashboard under Settings (changelog 2025-03-24: "create your API key from the Settings page").'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cloudpepper-io-openapi.yml
  type: http
- description: 'MCP clients connect by browser sign-in with a Cloudpepper account; the client is registered automatically (no client ID/secret). Available on Pro and Agency. Machine clients may instead send "Authorization: Bearer aak-..." (Agency only).'
  name: mcp-oauth-signin
  sources:
  - https://cloudpepper.io/docs/api-and-mcp/connect-claude-or-codex/
  surface: https://mcp.cloudpepper.io
  type: oauth2
slug: cloudpepper-io-authentication
source_filename: cloudpepper-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cloudpepper.io/docs/api-and-mcp/connect-claude-or-codex/\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cloudpepper-io-openapi.yml\n  description: 'Bearer token on every REST endpoint. Cloudpepper API keys (prefix\n    \"aak-\") are an Agency feature, created in the dashboard under Settings (changelog\n    2025-03-24: \"create your API key from the Settings page\").'\n- name: mcp-oauth-signin\n  type: oauth2\n  surface: https://mcp.cloudpepper.io\n  description: 'MCP clients connect by browser sign-in with a Cloudpepper account;\n    the client is registered automatically (no client ID/secret). Available on Pro\n    and Agency. Machine clients may instead send \"Authorization: Bearer aak-...\" (Agency\n    only).'\n  sources:\n  - https://cloudpepper.io/docs/api-and-mcp/connect-claude-or-codex/\ndocs: https://cloudpepper.io/docs/api-and-mcp/connect-claude-or-codex/\n"
source_yaml_url: https://artifacts.apis.io/cloudpepper-io/authentication/cloudpepper-io-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Odoo
- Hosting
- Cloud Control Panel
- ERP
- Managed Hosting
- DevOps
- Backups
- MCP
---
