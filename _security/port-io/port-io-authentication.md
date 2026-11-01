---
anonymous_access: false
api_key_in: []
api_specs:
- filename: port-io-blueprints-api-openapi.yml
  format: yaml
  label: Port Blueprints API
  slug: port-io-blueprints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-blueprints-api-openapi.yml
- filename: port-io-entities-api-openapi.yml
  format: yaml
  label: Port Entities API
  slug: port-io-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-entities-api-openapi.yml
- filename: port-io-action-runs-api-openapi.yml
  format: yaml
  label: Port Action Runs API
  slug: port-io-action-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-action-runs-api-openapi.yml
- filename: port-io-actions-api-openapi.yml
  format: yaml
  label: Port Actions API
  slug: port-io-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-actions-api-openapi.yml
- filename: port-io-ai-api-openapi.yml
  format: yaml
  label: Port AI API
  slug: port-io-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-ai-api-openapi.yml
- filename: port-io-apps-api-openapi.yml
  format: yaml
  label: Port Apps API
  slug: port-io-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-apps-api-openapi.yml
- filename: port-io-audit-api-openapi.yml
  format: yaml
  label: Port Audit API
  slug: port-io-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-audit-api-openapi.yml
- filename: port-io-authentication-authorization-api-openapi.yml
  format: yaml
  label: Port Authentication / Authorization API
  slug: port-io-authentication-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-authentication-authorization-api-openapi.yml
- filename: port-io-folders-api-openapi.yml
  format: yaml
  label: Port Folders API
  slug: port-io-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-folders-api-openapi.yml
- filename: port-io-integrations-api-openapi.yml
  format: yaml
  label: Port Integrations API
  slug: port-io-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-integrations-api-openapi.yml
- filename: port-io-migrations-api-openapi.yml
  format: yaml
  label: Port Migrations API
  slug: port-io-migrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-migrations-api-openapi.yml
- filename: port-io-organization-api-openapi.yml
  format: yaml
  label: Port Organization API
  slug: port-io-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-organization-api-openapi.yml
- filename: port-io-pages-api-openapi.yml
  format: yaml
  label: Port Pages API
  slug: port-io-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-pages-api-openapi.yml
- filename: port-io-scorecard-groups-api-openapi.yml
  format: yaml
  label: Port Scorecard Groups API
  slug: port-io-scorecard-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-scorecard-groups-api-openapi.yml
- filename: port-io-scorecards-api-openapi.yml
  format: yaml
  label: Port Scorecards API
  slug: port-io-scorecards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-scorecards-api-openapi.yml
- filename: port-io-teams-api-openapi.yml
  format: yaml
  label: Port Teams API
  slug: port-io-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-teams-api-openapi.yml
- filename: port-io-users-api-openapi.yml
  format: yaml
  label: Port Users API
  slug: port-io-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-users-api-openapi.yml
- filename: port-io-webhook-api-openapi.yml
  format: yaml
  label: Port Webhook API
  slug: port-io-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/port-io/openapi/port-io-webhook-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Port Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Port secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Port
provider_slug: port-io
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Port uses bearer tokens obtained from the Port application credentials panel.

    Tokens remain valid for 3 hours.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/port-io-openapi.yml
  type: http
slug: port-io-authentication
source_filename: port-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/port-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Port uses bearer tokens obtained from the Port application credentials panel.\n    Tokens remain valid for 3 hours.\n  sources:\n  - openapi/port-io-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/port-io/authentication/port-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Internal Developer Portal
- Service Catalog
- Self-Service Actions
- Platform Engineering
- Scorecards
- Developer Experience
- Developer Portal
---
