---
anonymous_access: false
api_key_in: []
api_specs:
- filename: abm-dev-campaigns-api-openapi.yml
  format: yaml
  label: abm-dev Campaigns API
  slug: abm-dev-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-campaigns-api-openapi.yml
- filename: abm-dev-crm-api-openapi.yml
  format: yaml
  label: abm-dev CRM API
  slug: abm-dev-crm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-crm-api-openapi.yml
- filename: abm-dev-enrichment-api-openapi.yml
  format: yaml
  label: abm-dev Enrichment API
  slug: abm-dev-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-enrichment-api-openapi.yml
- filename: abm-dev-enrichment-config-api-openapi.yml
  format: yaml
  label: abm-dev Enrichment Config API
  slug: abm-dev-enrichment-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-enrichment-config-api-openapi.yml
- filename: abm-dev-field-configuration-api-openapi.yml
  format: yaml
  label: abm-dev Field Configuration API
  slug: abm-dev-field-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-field-configuration-api-openapi.yml
- filename: abm-dev-health-api-openapi.yml
  format: yaml
  label: abm-dev Health API
  slug: abm-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-health-api-openapi.yml
- filename: abm-dev-organization-api-openapi.yml
  format: yaml
  label: abm-dev Organization API
  slug: abm-dev-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-organization-api-openapi.yml
- filename: abm-dev-people-finder-api-openapi.yml
  format: yaml
  label: abm-dev People Finder API
  slug: abm-dev-people-finder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-people-finder-api-openapi.yml
- filename: abm-dev-webhooks-api-openapi.yml
  format: yaml
  label: abm-dev Webhooks API
  slug: abm-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abm-dev/openapi/abm-dev-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Abm Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: abm-dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: abm-dev
provider_slug: abm-dev
scheme_count: 2
schemes:
- description: API key header for simple auth.
  in: header
  name: X-API-Key
  type: apiKey
- bearerFormat: JWT
  description: JWT token issued via Clerk.
  scheme: bearer
  type: http
slug: abm-dev-authentication
source_filename: abm-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: https://abm.dev/docs/concepts/authentication\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key header for simple auth.\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: JWT token issued via Clerk.\n"
source_yaml_url: https://artifacts.apis.io/abm-dev/authentication/abm-dev-authentication.yml
summary_line: 2 schemes
tags:
- Account-Based Marketing
- AI Agents
- Data Enrichment
- B2B
- Marketing API
---
