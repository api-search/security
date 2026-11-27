---
anonymous_access: false
api_key_in: []
api_specs:
- filename: flashdata-dev-account-api-openapi.yml
  format: yaml
  label: FlashData Account API
  slug: flashdata-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-account-api-openapi.yml
- filename: flashdata-dev-agent-connections-api-openapi.yml
  format: yaml
  label: FlashData Agent Connections API
  slug: flashdata-dev-agent-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-agent-connections-api-openapi.yml
- filename: flashdata-dev-api-keys-api-openapi.yml
  format: yaml
  label: FlashData API Keys API
  slug: flashdata-dev-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-api-keys-api-openapi.yml
- filename: flashdata-dev-auth-api-openapi.yml
  format: yaml
  label: FlashData Auth API
  slug: flashdata-dev-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-auth-api-openapi.yml
- filename: flashdata-dev-billing-api-openapi.yml
  format: yaml
  label: FlashData Billing API
  slug: flashdata-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-billing-api-openapi.yml
- filename: flashdata-dev-bulk-jobs-api-openapi.yml
  format: yaml
  label: FlashData Bulk Jobs API
  slug: flashdata-dev-bulk-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-bulk-jobs-api-openapi.yml
- filename: flashdata-dev-catalog-api-openapi.yml
  format: yaml
  label: FlashData Catalog API
  slug: flashdata-dev-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-catalog-api-openapi.yml
- filename: flashdata-dev-credits-api-openapi.yml
  format: yaml
  label: FlashData Credits API
  slug: flashdata-dev-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-credits-api-openapi.yml
- filename: flashdata-dev-data-queries-api-openapi.yml
  format: yaml
  label: FlashData Data Queries API
  slug: flashdata-dev-data-queries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-data-queries-api-openapi.yml
- filename: flashdata-dev-delivery-api-openapi.yml
  format: yaml
  label: FlashData Delivery API
  slug: flashdata-dev-delivery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-delivery-api-openapi.yml
- filename: flashdata-dev-jobs-api-openapi.yml
  format: yaml
  label: FlashData Jobs API
  slug: flashdata-dev-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-jobs-api-openapi.yml
- filename: flashdata-dev-onboarding-api-openapi.yml
  format: yaml
  label: FlashData Onboarding API
  slug: flashdata-dev-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-onboarding-api-openapi.yml
- filename: flashdata-dev-overview-api-openapi.yml
  format: yaml
  label: FlashData Overview API
  slug: flashdata-dev-overview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-overview-api-openapi.yml
- filename: flashdata-dev-playground-api-openapi.yml
  format: yaml
  label: FlashData Playground API
  slug: flashdata-dev-playground-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-playground-api-openapi.yml
- filename: flashdata-dev-system-api-openapi.yml
  format: yaml
  label: FlashData System API
  slug: flashdata-dev-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-system-api-openapi.yml
- filename: flashdata-dev-trial-credits-api-openapi.yml
  format: yaml
  label: FlashData Trial Credits API
  slug: flashdata-dev-trial-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flashdata-dev/openapi/flashdata-dev-trial-credits-api-openapi.yml
auth_types: []
description: Authentication methods for FlashData
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: FlashData Authentication
name_suffix: Authentication
oauth_flows: []
overview: FlashData declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FlashData
provider_slug: flashdata-dev
scheme_count: 2
schemes:
- evidence: REST requests use X-API-Key with a trial or owner key.
  header: X-API-Key
  how_to_obtain: Create an API key in the FlashData console (API Keys) or obtain a temporary trial key via the agent onboarding flow.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: Use a host configured for FlashData OAuth. The account owner completes signup or sign-in and consent in the browser; the host saves the tokens.
  header: Authorization
  how_to_obtain: Connect through MCP OAuth; the host obtains, stores, and refreshes the Bearer token after user consent.
  location: header
  name: Authorization
  type: oauth2
slug: flashdata-dev-authentication
source_filename: flashdata-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://flashdata.dev/auth.md
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://flashdata.dev/auth.md\nsources:\n- https://flashdata.dev/auth.md\n- https://flashdata.dev/docs/guides/headers-and-authentication/reference.md\n- https://flashdata.dev/docs/guides/api-keys-and-permissions/reference.md\n- https://flashdata.dev/docs/guides/agent-access/reference.md\ndescription: Authentication methods for FlashData\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: REST requests use X-API-Key with a trial or owner key.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an API key in the FlashData console (API Keys) or obtain a temporary trial key via the agent onboarding flow.\n- type: oauth2\n  name: Authorization\n  evidence: Use a host configured for FlashData OAuth. The account owner completes signup or sign-in and consent in the browser; the host saves\n    the tokens.\n  location: header\n  header: Authorization\n  how_to_obtain:\
  \ Connect through MCP OAuth; the host obtains, stores, and refreshes the Bearer token after user consent.\ndocs: https://flashdata.dev/auth.md\n"
source_yaml_url: https://artifacts.apis.io/flashdata-dev/authentication/flashdata-dev-authentication.yml
summary_line: 2 schemes
tags:
- SERP
- Video Metadata
- Media Download
- Cloud Storage
- Developer Tools
- AI Agents
---
