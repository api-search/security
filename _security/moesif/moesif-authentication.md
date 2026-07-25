---
api_key_in: []
api_specs:
- filename: moesif-applications-api-openapi.yml
  format: yaml
  label: Moesif Applications API
  slug: moesif-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-applications-api-openapi.yml
- filename: moesif-balance-transactions-api-openapi.yml
  format: yaml
  label: Moesif Balance Transactions API
  slug: moesif-balance-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-balance-transactions-api-openapi.yml
- filename: moesif-billing-meters-api-openapi.yml
  format: yaml
  label: Moesif Billing Meters API
  slug: moesif-billing-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-billing-meters-api-openapi.yml
- filename: moesif-billing-reports-api-openapi.yml
  format: yaml
  label: Moesif Billing Reports API
  slug: moesif-billing-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-billing-reports-api-openapi.yml
- filename: moesif-cohorts-api-openapi.yml
  format: yaml
  label: Moesif Cohorts API
  slug: moesif-cohorts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-cohorts-api-openapi.yml
- filename: moesif-companies-api-openapi.yml
  format: yaml
  label: Moesif Companies API
  slug: moesif-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-companies-api-openapi.yml
- filename: moesif-dashboards-api-openapi.yml
  format: yaml
  label: Moesif Dashboards API
  slug: moesif-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-dashboards-api-openapi.yml
- filename: moesif-email-templates-api-openapi.yml
  format: yaml
  label: Moesif Email Templates API
  slug: moesif-email-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-email-templates-api-openapi.yml
- filename: moesif-governance-rules-api-openapi.yml
  format: yaml
  label: Moesif Governance Rules API
  slug: moesif-governance-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-governance-rules-api-openapi.yml
- filename: moesif-metrics-api-openapi.yml
  format: yaml
  label: Moesif Metrics API
  slug: moesif-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-metrics-api-openapi.yml
- filename: moesif-product-catalog-api-openapi.yml
  format: yaml
  label: Moesif Product Catalog API
  slug: moesif-product-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-product-catalog-api-openapi.yml
- filename: moesif-properties-api-openapi.yml
  format: yaml
  label: Moesif Properties API
  slug: moesif-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-properties-api-openapi.yml
- filename: moesif-subscriptions-api-openapi.yml
  format: yaml
  label: Moesif Subscriptions API
  slug: moesif-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-subscriptions-api-openapi.yml
- filename: moesif-users-api-openapi.yml
  format: yaml
  label: Moesif Users API
  slug: moesif-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-users-api-openapi.yml
- filename: moesif-workspaces-api-openapi.yml
  format: yaml
  label: Moesif Workspaces API
  slug: moesif-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-workspaces-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Moesif Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Moesif secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Moesif
provider_slug: moesif
scheme_count: 1
schemes:
- description: "Your Management API token must be added to the request _Authorization_ header using the following format:\n\n `Authorization: Bearer [example key]`"
  flows:
  - flow: password
    scopes: 41
    tokenUrl: https://api.moesif.com/v1/:orgId/oauth/access_tokens
  name: managementAPIToken
  sources:
  - openapi/moesif-openapi.json
  - openapi/moesif-openapi.yml
  type: oauth2
slug: moesif-authentication
source_filename: moesif-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moesif-openapi.json, openapi/moesif-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: managementAPIToken\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://api.moesif.com/v1/:orgId/oauth/access_tokens\n    scopes: 41\n  description: |-\n    Your Management API token must be added to the request _Authorization_ header using the following format:\n\n     `Authorization: Bearer [example key]`\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/authentication/moesif-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Monitoring
- Monetization
- Governance
- Observability
- Billing
- AI Agents
- LLM Analytics
- OpenTelemetry
- Developer Portal
- Platform
- Insights
---
