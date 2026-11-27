---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: georgiacommons-org-bulk-api-openapi.yml
  format: yaml
  label: Georgia Commons Bulk API
  slug: georgiacommons-org-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiacommons-org/openapi/georgiacommons-org-bulk-api-openapi.yml
- filename: georgiacommons-org-chat-api-openapi.yml
  format: yaml
  label: Georgia Commons Chat API
  slug: georgiacommons-org-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiacommons-org/openapi/georgiacommons-org-chat-api-openapi.yml
- filename: georgiacommons-org-coverage-api-openapi.yml
  format: yaml
  label: Georgia Commons Coverage API
  slug: georgiacommons-org-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiacommons-org/openapi/georgiacommons-org-coverage-api-openapi.yml
- filename: georgiacommons-org-documents-api-openapi.yml
  format: yaml
  label: Georgia Commons Documents API
  slug: georgiacommons-org-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiacommons-org/openapi/georgiacommons-org-documents-api-openapi.yml
- filename: georgiacommons-org-georgia-commons-api-api-openapi.yml
  format: yaml
  label: Georgia Commons Georgia Commons API
  slug: georgiacommons-org-georgia-commons-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiacommons-org/openapi/georgiacommons-org-georgia-commons-api-api-openapi.yml
- filename: georgiacommons-org-health-api-openapi.yml
  format: yaml
  label: Georgia Commons Health API
  slug: georgiacommons-org-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiacommons-org/openapi/georgiacommons-org-health-api-openapi.yml
- filename: georgiacommons-org-search-api-openapi.yml
  format: yaml
  label: Georgia Commons Search API
  slug: georgiacommons-org-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiacommons-org/openapi/georgiacommons-org-search-api-openapi.yml
- filename: georgiacommons-org-sitemap-api-openapi.yml
  format: yaml
  label: Georgia Commons Sitemap API
  slug: georgiacommons-org-sitemap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiacommons-org/openapi/georgiacommons-org-sitemap-api-openapi.yml
- filename: georgiacommons-org-status-api-openapi.yml
  format: yaml
  label: Georgia Commons Status API
  slug: georgiacommons-org-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiacommons-org/openapi/georgiacommons-org-status-api-openapi.yml
- filename: georgiacommons-org-usage-api-openapi.yml
  format: yaml
  label: Georgia Commons Usage API
  slug: georgiacommons-org-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiacommons-org/openapi/georgiacommons-org-usage-api-openapi.yml
- filename: georgiacommons-org-verify-api-openapi.yml
  format: yaml
  label: Georgia Commons Verify API
  slug: georgiacommons-org-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/georgiacommons-org/openapi/georgiacommons-org-verify-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Georgia Commons Authentication
name_suffix: Authentication
oauth_flows: []
overview: Georgia Commons secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Georgia Commons
provider_slug: georgiacommons-org
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/georgiacommons-org-openapi.json
  type: apiKey
slug: georgiacommons-org-authentication
source_filename: georgiacommons-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/georgiacommons-org-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/georgiacommons-org-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/georgiacommons-org/authentication/georgiacommons-org-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Bills
- Court Opinions
- Code
- Meetings
- Public Data
- Government Documents
- AI Assistant
---
