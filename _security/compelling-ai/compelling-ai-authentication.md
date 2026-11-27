---
anonymous_access: false
api_key_in: []
api_specs:
- filename: compelling-ai-accounts-api-openapi.yml
  format: yaml
  label: Compelling Accounts API
  slug: compelling-ai-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compelling-ai/openapi/compelling-ai-accounts-api-openapi.yml
- filename: compelling-ai-contacts-api-openapi.yml
  format: yaml
  label: Compelling Contacts API
  slug: compelling-ai-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compelling-ai/openapi/compelling-ai-contacts-api-openapi.yml
- filename: compelling-ai-credits-api-openapi.yml
  format: yaml
  label: Compelling Credits API
  slug: compelling-ai-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compelling-ai/openapi/compelling-ai-credits-api-openapi.yml
- filename: compelling-ai-exports-api-openapi.yml
  format: yaml
  label: Compelling Exports API
  slug: compelling-ai-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compelling-ai/openapi/compelling-ai-exports-api-openapi.yml
- filename: compelling-ai-integrations-api-openapi.yml
  format: yaml
  label: Compelling Integrations API
  slug: compelling-ai-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compelling-ai/openapi/compelling-ai-integrations-api-openapi.yml
- filename: compelling-ai-jobs-api-openapi.yml
  format: yaml
  label: Compelling Jobs API
  slug: compelling-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compelling-ai/openapi/compelling-ai-jobs-api-openapi.yml
- filename: compelling-ai-lists-api-openapi.yml
  format: yaml
  label: Compelling Lists API
  slug: compelling-ai-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compelling-ai/openapi/compelling-ai-lists-api-openapi.yml
- filename: compelling-ai-search-api-openapi.yml
  format: yaml
  label: Compelling Search API
  slug: compelling-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compelling-ai/openapi/compelling-ai-search-api-openapi.yml
- filename: compelling-ai-views-api-openapi.yml
  format: yaml
  label: Compelling Views API
  slug: compelling-ai-views-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compelling-ai/openapi/compelling-ai-views-api-openapi.yml
- filename: compelling-ai-workflows-api-openapi.yml
  format: yaml
  label: Compelling Workflows API
  slug: compelling-ai-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compelling-ai/openapi/compelling-ai-workflows-api-openapi.yml
- filename: compelling-ai-workspaces-api-openapi.yml
  format: yaml
  label: Compelling Workspaces API
  slug: compelling-ai-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compelling-ai/openapi/compelling-ai-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Compelling Authentication
name_suffix: Authentication
oauth_flows: []
overview: Compelling secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Compelling
provider_slug: compelling-ai
scheme_count: 1
schemes:
- description: 'API key issued from your workspace settings. Pass as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/compelling-ai-openapi.yml
  type: http
slug: compelling-ai-authentication
source_filename: compelling-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/compelling-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key issued from your workspace settings. Pass as `Authorization: Bearer\n    <token>`.'\n  sources:\n  - openapi/compelling-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/compelling-ai/authentication/compelling-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Sales Intelligence
- Contact Enrichment
- Artificial Intelligence
- CRM
- Lead Generation
- GDPR
- MCP
---
