---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mcphost-dev-assets-api-openapi.yml
  format: yaml
  label: mcphost Assets API
  slug: mcphost-dev-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-assets-api-openapi.yml
- filename: mcphost-dev-billing-api-openapi.yml
  format: yaml
  label: mcphost Billing API
  slug: mcphost-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-billing-api-openapi.yml
- filename: mcphost-dev-claim-api-openapi.yml
  format: yaml
  label: mcphost Claim API
  slug: mcphost-dev-claim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-claim-api-openapi.yml
- filename: mcphost-dev-help-api-openapi.yml
  format: yaml
  label: mcphost Help API
  slug: mcphost-dev-help-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-help-api-openapi.yml
- filename: mcphost-dev-oauth-api-openapi.yml
  format: yaml
  label: mcphost OAuth API
  slug: mcphost-dev-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-oauth-api-openapi.yml
- filename: mcphost-dev-onboarding-api-openapi.yml
  format: yaml
  label: mcphost Onboarding API
  slug: mcphost-dev-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-onboarding-api-openapi.yml
- filename: mcphost-dev-public-tool-api-openapi.yml
  format: yaml
  label: mcphost Public Tool API
  slug: mcphost-dev-public-tool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-public-tool-api-openapi.yml
- filename: mcphost-dev-status-api-openapi.yml
  format: yaml
  label: mcphost Status API
  slug: mcphost-dev-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-status-api-openapi.yml
- filename: mcphost-dev-webhooks-api-openapi.yml
  format: yaml
  label: mcphost Webhooks API
  slug: mcphost-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-webhooks-api-openapi.yml
- filename: mcphost-dev-well-known-api-openapi.yml
  format: yaml
  label: mcphost Well Known API
  slug: mcphost-dev-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcphost-dev/openapi/mcphost-dev-well-known-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: mcphost Authentication
name_suffix: Authentication
oauth_flows: []
overview: mcphost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: mcphost
provider_slug: mcphost-dev
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mcphost-dev-openapi.json
  type: http
slug: mcphost-dev-authentication
source_filename: mcphost-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/mcphost-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/mcphost-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mcphost-dev/authentication/mcphost-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Hosting
- MCP
- Tools
- Platform
---
