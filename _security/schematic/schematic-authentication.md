---
api_key_in:
- header
api_specs:
- filename: schematic-accesstokens-api-openapi.yml
  format: yaml
  label: Schematic accesstokens API
  slug: schematic-accesstokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-accesstokens-api-openapi.yml
- filename: schematic-accounts-api-openapi.yml
  format: yaml
  label: Schematic accounts API
  slug: schematic-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-accounts-api-openapi.yml
- filename: schematic-billing-api-openapi.yml
  format: yaml
  label: Schematic billing API
  slug: schematic-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-billing-api-openapi.yml
- filename: schematic-checkout-api-openapi.yml
  format: yaml
  label: Schematic checkout API
  slug: schematic-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-checkout-api-openapi.yml
- filename: schematic-companies-api-openapi.yml
  format: yaml
  label: Schematic companies API
  slug: schematic-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-companies-api-openapi.yml
- filename: schematic-components-api-openapi.yml
  format: yaml
  label: Schematic components API
  slug: schematic-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-components-api-openapi.yml
- filename: schematic-componentspublic-api-openapi.yml
  format: yaml
  label: Schematic componentspublic API
  slug: schematic-componentspublic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-componentspublic-api-openapi.yml
- filename: schematic-credits-api-openapi.yml
  format: yaml
  label: Schematic credits API
  slug: schematic-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-credits-api-openapi.yml
- filename: schematic-dataexports-api-openapi.yml
  format: yaml
  label: Schematic dataexports API
  slug: schematic-dataexports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-dataexports-api-openapi.yml
- filename: schematic-entitlements-api-openapi.yml
  format: yaml
  label: Schematic entitlements API
  slug: schematic-entitlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-entitlements-api-openapi.yml
- filename: schematic-events-api-openapi.yml
  format: yaml
  label: Schematic events API
  slug: schematic-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-events-api-openapi.yml
- filename: schematic-features-api-openapi.yml
  format: yaml
  label: Schematic features API
  slug: schematic-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-features-api-openapi.yml
- filename: schematic-insights-api-openapi.yml
  format: yaml
  label: Schematic insights API
  slug: schematic-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-insights-api-openapi.yml
- filename: schematic-integrationsapi-api-openapi.yml
  format: yaml
  label: Schematic integrationsapi API
  slug: schematic-integrationsapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-integrationsapi-api-openapi.yml
- filename: schematic-planbundle-api-openapi.yml
  format: yaml
  label: Schematic planbundle API
  slug: schematic-planbundle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-planbundle-api-openapi.yml
- filename: schematic-plangroups-api-openapi.yml
  format: yaml
  label: Schematic plangroups API
  slug: schematic-plangroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-plangroups-api-openapi.yml
- filename: schematic-planmigrations-api-openapi.yml
  format: yaml
  label: Schematic planmigrations API
  slug: schematic-planmigrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-planmigrations-api-openapi.yml
- filename: schematic-plans-api-openapi.yml
  format: yaml
  label: Schematic plans API
  slug: schematic-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-plans-api-openapi.yml
- filename: schematic-scheduledcheckout-api-openapi.yml
  format: yaml
  label: Schematic scheduledcheckout API
  slug: schematic-scheduledcheckout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-scheduledcheckout-api-openapi.yml
- filename: schematic-webhooks-api-openapi.yml
  format: yaml
  label: Schematic webhooks API
  slug: schematic-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/openapi/schematic-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Schematic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Schematic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Schematic
provider_slug: schematic
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Schematic-Api-Key
  sources:
  - openapi/schematic-openapi.yml
  type: apiKey
slug: schematic-authentication
source_filename: schematic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/schematic-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Schematic-Api-Key\n  sources:\n  - openapi/schematic-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/authentication/schematic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Billing
- Entitlements
- Feature Flags
- Feature Management
- FinOps
- Metering
- Pricing
- Software-as-a-Service
---
