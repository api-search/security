---
anonymous_access: false
api_key_in: []
api_specs:
- filename: 0latency-ai-admin-api-openapi.yml
  format: yaml
  label: 0latency-ai Admin API
  slug: 0latency-ai-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-admin-api-openapi.yml
- filename: 0latency-ai-api-keys-api-openapi.yml
  format: yaml
  label: 0latency-ai Api Keys API
  slug: 0latency-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-api-keys-api-openapi.yml
- filename: 0latency-ai-auth-api-openapi.yml
  format: yaml
  label: 0latency-ai Auth API
  slug: 0latency-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-auth-api-openapi.yml
- filename: 0latency-ai-billing-api-openapi.yml
  format: yaml
  label: 0latency-ai Billing API
  slug: 0latency-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-billing-api-openapi.yml
- filename: 0latency-ai-criteria-api-openapi.yml
  format: yaml
  label: 0latency-ai Criteria API
  slug: 0latency-ai-criteria-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-criteria-api-openapi.yml
- filename: 0latency-ai-dashboard-api-openapi.yml
  format: yaml
  label: 0latency-ai Dashboard API
  slug: 0latency-ai-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-dashboard-api-openapi.yml
- filename: 0latency-ai-extract-api-openapi.yml
  format: yaml
  label: 0latency-ai Extract API
  slug: 0latency-ai-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-extract-api-openapi.yml
- filename: 0latency-ai-graph-api-openapi.yml
  format: yaml
  label: 0latency-ai Graph API
  slug: 0latency-ai-graph-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-graph-api-openapi.yml
- filename: 0latency-ai-health-api-openapi.yml
  format: yaml
  label: 0latency-ai Health API
  slug: 0latency-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-health-api-openapi.yml
- filename: 0latency-ai-memories-api-openapi.yml
  format: yaml
  label: 0latency-ai Memories API
  slug: 0latency-ai-memories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-memories-api-openapi.yml
- filename: 0latency-ai-org-api-openapi.yml
  format: yaml
  label: 0latency-ai Org API
  slug: 0latency-ai-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-org-api-openapi.yml
- filename: 0latency-ai-recall-api-openapi.yml
  format: yaml
  label: 0latency-ai Recall API
  slug: 0latency-ai-recall-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-recall-api-openapi.yml
- filename: 0latency-ai-schemas-api-openapi.yml
  format: yaml
  label: 0latency-ai Schemas API
  slug: 0latency-ai-schemas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-schemas-api-openapi.yml
- filename: 0latency-ai-tenant-info-api-openapi.yml
  format: yaml
  label: 0latency-ai Tenant Info API
  slug: 0latency-ai-tenant-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-tenant-info-api-openapi.yml
- filename: 0latency-ai-usage-api-openapi.yml
  format: yaml
  label: 0latency-ai Usage API
  slug: 0latency-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-usage-api-openapi.yml
- filename: 0latency-ai-webhooks-api-openapi.yml
  format: yaml
  label: 0latency-ai Webhooks API
  slug: 0latency-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/0latency-ai/openapi/0latency-ai-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: 0Latency Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: 0latency-ai declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: 0latency-ai
provider_slug: 0latency-ai
scheme_count: 3
schemes:
- description: Redirect to GitHub OAuth consent screen
  flow: authorizationCode
  name: GitHub OAuth
  type: oauth2
- description: Redirect to Google OAuth consent screen
  flow: authorizationCode
  name: Google OAuth
  type: oauth2
- description: Register and login with email and password
  name: Email Register/Login
  type: email
slug: 0latency-ai-authentication
source_filename: 0latency-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/0latency-ai-openapi.json\nschemes:\n  - type: \"oauth2\"\n    name: \"GitHub OAuth\"\n    flow: \"authorizationCode\"\n    description: \"Redirect to GitHub OAuth consent screen\"\n  - type: \"oauth2\"\n    name: \"Google OAuth\"\n    flow: \"authorizationCode\"\n    description: \"Redirect to Google OAuth consent screen\"\n  - type: \"email\"\n    name: \"Email Register/Login\"\n    description: \"Register and login with email and password\"\n"
source_yaml_url: https://artifacts.apis.io/0latency-ai/authentication/0latency-ai-authentication.yml
summary_line: 3 schemes
tags:
- Company
- AI
- Memory
- Agent
- Platform
- API
---
