---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: onboard-io-activity-api-openapi.yml
  format: yaml
  label: Onboard Activity API
  slug: onboard-io-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-activity-api-openapi.yml
- filename: onboard-io-assets-api-openapi.yml
  format: yaml
  label: Onboard Assets API
  slug: onboard-io-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-assets-api-openapi.yml
- filename: onboard-io-bots-api-openapi.yml
  format: yaml
  label: Onboard Bots API
  slug: onboard-io-bots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-bots-api-openapi.yml
- filename: onboard-io-comments-api-openapi.yml
  format: yaml
  label: Onboard Comments API
  slug: onboard-io-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-comments-api-openapi.yml
- filename: onboard-io-communication-records-api-openapi.yml
  format: yaml
  label: Onboard Communication Records API
  slug: onboard-io-communication-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-communication-records-api-openapi.yml
- filename: onboard-io-compliance-api-openapi.yml
  format: yaml
  label: Onboard Compliance API
  slug: onboard-io-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-compliance-api-openapi.yml
- filename: onboard-io-conversations-api-openapi.yml
  format: yaml
  label: Onboard Conversations API
  slug: onboard-io-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-conversations-api-openapi.yml
- filename: onboard-io-custom-api-openapi.yml
  format: yaml
  label: Onboard Custom API
  slug: onboard-io-custom-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-custom-api-openapi.yml
- filename: onboard-io-email-api-openapi.yml
  format: yaml
  label: Onboard Email API
  slug: onboard-io-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-email-api-openapi.yml
- filename: onboard-io-hooks-api-openapi.yml
  format: yaml
  label: Onboard Hooks API
  slug: onboard-io-hooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-hooks-api-openapi.yml
- filename: onboard-io-knowledge-base-api-openapi.yml
  format: yaml
  label: Onboard Knowledge Base API
  slug: onboard-io-knowledge-base-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-knowledge-base-api-openapi.yml
- filename: onboard-io-map-api-openapi.yml
  format: yaml
  label: Onboard Map API
  slug: onboard-io-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-map-api-openapi.yml
- filename: onboard-io-platform-api-openapi.yml
  format: yaml
  label: Onboard Platform API
  slug: onboard-io-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-platform-api-openapi.yml
- filename: onboard-io-stats-api-openapi.yml
  format: yaml
  label: Onboard Stats API
  slug: onboard-io-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-stats-api-openapi.yml
- filename: onboard-io-workflows-api-openapi.yml
  format: yaml
  label: Onboard Workflows API
  slug: onboard-io-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onboard-io/openapi/onboard-io-workflows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Onboard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Onboard secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Onboard
provider_slug: onboard-io
scheme_count: 1
schemes:
- description: 'API key authentication. Format: Your API key (no "Token" prefix needed)'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/onboard-io-openapi.json
  type: apiKey
slug: onboard-io-authentication
source_filename: onboard-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/onboard-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key authentication. Format: Your API key (no \"Token\" prefix needed)'\n  sources:\n  - openapi/onboard-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/onboard-io/authentication/onboard-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Customer Onboarding
- Software-as-a-Service
- B2B
- Integration
- Artificial Intelligence
---
