---
anonymous_access: false
api_key_in: []
api_specs:
- filename: arkrel-com-account-data-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Account Data API
  slug: arkrel-com-account-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-account-data-api-openapi.yml
- filename: arkrel-com-auth-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Auth API
  slug: arkrel-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-auth-api-openapi.yml
- filename: arkrel-com-billing-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Billing API
  slug: arkrel-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-billing-api-openapi.yml
- filename: arkrel-com-businesses-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Businesses API
  slug: arkrel-com-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-businesses-api-openapi.yml
- filename: arkrel-com-category-rules-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Category Rules API
  slug: arkrel-com-category-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-category-rules-api-openapi.yml
- filename: arkrel-com-chart-of-accounts-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Chart Of Accounts API
  slug: arkrel-com-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-chart-of-accounts-api-openapi.yml
- filename: arkrel-com-connections-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Connections API
  slug: arkrel-com-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-connections-api-openapi.yml
- filename: arkrel-com-documents-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Documents API
  slug: arkrel-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-documents-api-openapi.yml
- filename: arkrel-com-mcp-api-openapi.yml
  format: yaml
  label: Conecta Media LLC MCP API
  slug: arkrel-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-mcp-api-openapi.yml
- filename: arkrel-com-ops-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Ops API
  slug: arkrel-com-ops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-ops-api-openapi.yml
- filename: arkrel-com-schemas-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Schemas API
  slug: arkrel-com-schemas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-schemas-api-openapi.yml
- filename: arkrel-com-settings-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Settings API
  slug: arkrel-com-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-settings-api-openapi.yml
- filename: arkrel-com-statement-sets-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Statement Sets API
  slug: arkrel-com-statement-sets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-statement-sets-api-openapi.yml
- filename: arkrel-com-tax-report-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Tax Report API
  slug: arkrel-com-tax-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-tax-report-api-openapi.yml
- filename: arkrel-com-tax-years-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Tax Years API
  slug: arkrel-com-tax-years-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-tax-years-api-openapi.yml
- filename: arkrel-com-usage-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Usage API
  slug: arkrel-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-usage-api-openapi.yml
- filename: arkrel-com-webhooks-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Webhooks API
  slug: arkrel-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-webhooks-api-openapi.yml
- filename: arkrel-com-year-overview-api-openapi.yml
  format: yaml
  label: Conecta Media LLC Year Overview API
  slug: arkrel-com-year-overview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkrel-com/openapi/arkrel-com-year-overview-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Arkrel Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conecta Media LLC declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Conecta Media LLC
provider_slug: arkrel-com
scheme_count: 1
schemes:
- description: Bearer API keys used for REST API authentication. Keys are created in the Dashboard under API keys. Full key shown once; stored as hash.
  expiry:
    description: Optional expiry set at creation (30 days, 90 days, or 1 year). Expired keys stop authenticating like revoked keys.
  scopes:
  - description: 'Can call every endpoint: upload/delete documents, create/delete webhooks and schemas.'
    name: write
  - description: Read‑only access to list/fetch documents, schemas, webhooks, usage. Returns 403 FORBIDDEN for write operations.
    name: read
  type: bearer
slug: arkrel-com-authentication
source_filename: arkrel-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://arkrel.com/docs/authentication\nschemes:\n  - type: bearer\n    description: \"Bearer API keys used for REST API authentication. Keys are created in the Dashboard under API keys. Full key shown once; stored as hash.\"\n    scopes:\n      - name: write\n        description: \"Can call every endpoint: upload/delete documents, create/delete webhooks and schemas.\"\n      - name: read\n        description: \"Read‑only access to list/fetch documents, schemas, webhooks, usage. Returns 403 FORBIDDEN for write operations.\"\n    expiry:\n      description: \"Optional expiry set at creation (30 days, 90 days, or 1 year). Expired keys stop authenticating like revoked keys.\"\n"
source_yaml_url: https://artifacts.apis.io/arkrel-com/authentication/arkrel-com-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Bookkeeping
- Tax
- Software-as-a-Service
- Self-Employed
---
