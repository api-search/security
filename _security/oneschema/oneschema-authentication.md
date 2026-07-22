---
api_key_in:
- header
api_specs:
- filename: oneschema-importer-embeds-openapi.yml
  format: yaml
  label: OneSchema Importer Embeds API
  slug: oneschema-importer-embeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-importer-embeds-openapi.yml
- filename: oneschema-templates-openapi.yml
  format: yaml
  label: OneSchema Templates API
  slug: oneschema-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-templates-openapi.yml
- filename: oneschema-sheets-openapi.yml
  format: yaml
  label: OneSchema Sheets API
  slug: oneschema-sheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-sheets-openapi.yml
- filename: oneschema-workspaces-openapi.yml
  format: yaml
  label: OneSchema Workspaces API
  slug: oneschema-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-workspaces-openapi.yml
- filename: oneschema-multi-filefeeds-openapi.yml
  format: yaml
  label: OneSchema Multi FileFeeds API
  slug: oneschema-multi-filefeeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-multi-filefeeds-openapi.yml
- filename: oneschema-filefeeds-openapi.yml
  format: yaml
  label: OneSchema FileFeeds API
  slug: oneschema-filefeeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-filefeeds-openapi.yml
- filename: oneschema-importer-webhooks-openapi.yml
  format: yaml
  label: OneSchema Importer Webhooks API
  slug: oneschema-importer-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-importer-webhooks-openapi.yml
- filename: oneschema-event-webhooks-openapi.yml
  format: yaml
  label: OneSchema Event Webhooks API
  slug: oneschema-event-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-event-webhooks-openapi.yml
- filename: oneschema-code-hooks-legacy-openapi.yml
  format: yaml
  label: OneSchema Code Hooks (Legacy) API
  slug: oneschema-code-hooks-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-code-hooks-legacy-openapi.yml
- filename: oneschema-s3-accounts-openapi.yml
  format: yaml
  label: OneSchema S3 Accounts API
  slug: oneschema-s3-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-s3-accounts-openapi.yml
- filename: oneschema-sftp-accounts-openapi.yml
  format: yaml
  label: OneSchema SFTP Accounts API
  slug: oneschema-sftp-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-sftp-accounts-openapi.yml
- filename: oneschema-aws-secrets-manager-openapi.yml
  format: yaml
  label: OneSchema AWS Secrets Manager API
  slug: oneschema-aws-secrets-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-aws-secrets-manager-openapi.yml
- filename: oneschema-azure-key-vault-openapi.yml
  format: yaml
  label: OneSchema Azure Key Vault API
  slug: oneschema-azure-key-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-azure-key-vault-openapi.yml
- filename: oneschema-mcp-server-openapi.yml
  format: yaml
  label: OneSchema MCP Server API
  slug: oneschema-mcp-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/openapi/oneschema-mcp-server-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Oneschema Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oneschema secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oneschema
provider_slug: oneschema
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/oneschema-aws-secrets-manager-openapi.yml
  - openapi/oneschema-azure-key-vault-openapi.yml
  - openapi/oneschema-code-hooks-legacy-openapi.yml
  - openapi/oneschema-event-webhooks-openapi.yml
  - openapi/oneschema-filefeeds-openapi.yml
  - openapi/oneschema-importer-embeds-openapi.yml
  - openapi/oneschema-importer-webhooks-openapi.yml
  - openapi/oneschema-mcp-server-openapi.yml
  - openapi/oneschema-multi-filefeeds-openapi.yml
  - openapi/oneschema-s3-accounts-openapi.yml
  - openapi/oneschema-sftp-accounts-openapi.yml
  - openapi/oneschema-sheets-openapi.yml
  - openapi/oneschema-templates-openapi.yml
  - openapi/oneschema-workspaces-openapi.yml
  type: apiKey
slug: oneschema-authentication
source_filename: oneschema-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/oneschema-aws-secrets-manager-openapi.yml, openapi/oneschema-azure-key-vault-openapi.yml,\n  openapi/oneschema-code-hooks-legacy-openapi.yml, openapi/oneschema-event-webhooks-openapi.yml,\n  openapi/oneschema-filefeeds-openapi.yml, openapi/oneschema-importer-embeds-openapi.yml, openapi/oneschema-importer-webhooks-openapi.yml,\n  openapi/oneschema-mcp-server-openapi.yml, openapi/oneschema-multi-filefeeds-openapi.yml, openapi/oneschema-s3-accounts-openapi.yml,\n  openapi/oneschema-sftp-accounts-openapi.yml, openapi/oneschema-sheets-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/oneschema-aws-secrets-manager-openapi.yml\n  - openapi/oneschema-azure-key-vault-openapi.yml\n  - openapi/oneschema-code-hooks-legacy-openapi.yml\n  - openapi/oneschema-event-webhooks-openapi.yml\n  - openapi/oneschema-filefeeds-openapi.yml\n\
  \  - openapi/oneschema-importer-embeds-openapi.yml\n  - openapi/oneschema-importer-webhooks-openapi.yml\n  - openapi/oneschema-mcp-server-openapi.yml\n  - openapi/oneschema-multi-filefeeds-openapi.yml\n  - openapi/oneschema-s3-accounts-openapi.yml\n  - openapi/oneschema-sftp-accounts-openapi.yml\n  - openapi/oneschema-sheets-openapi.yml\n  - openapi/oneschema-templates-openapi.yml\n  - openapi/oneschema-workspaces-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oneschema/refs/heads/main/authentication/oneschema-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data Onboarding
- CSV Import
- Data Validation
- File Processing
- ETL
- Data Integration
- Embeddable UI
- Spreadsheets
- Developer Tools
- AI Data Transformation
---
