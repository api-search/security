---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getfinero-com-aging-api-openapi.yml
  format: yaml
  label: Finero Aging API
  slug: getfinero-com-aging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getfinero-com/openapi/getfinero-com-aging-api-openapi.yml
- filename: getfinero-com-api-context-api-openapi.yml
  format: yaml
  label: Finero API context API
  slug: getfinero-com-api-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getfinero-com/openapi/getfinero-com-api-context-api-openapi.yml
- filename: getfinero-com-erp-sync-api-openapi.yml
  format: yaml
  label: Finero ERP sync API
  slug: getfinero-com-erp-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getfinero-com/openapi/getfinero-com-erp-sync-api-openapi.yml
- filename: getfinero-com-integrations-api-openapi.yml
  format: yaml
  label: Finero Integrations API
  slug: getfinero-com-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getfinero-com/openapi/getfinero-com-integrations-api-openapi.yml
- filename: getfinero-com-invoices-api-openapi.yml
  format: yaml
  label: Finero Invoices API
  slug: getfinero-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getfinero-com/openapi/getfinero-com-invoices-api-openapi.yml
- filename: getfinero-com-payment-links-api-openapi.yml
  format: yaml
  label: Finero Payment links API
  slug: getfinero-com-payment-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getfinero-com/openapi/getfinero-com-payment-links-api-openapi.yml
- filename: getfinero-com-payments-api-openapi.yml
  format: yaml
  label: Finero Payments API
  slug: getfinero-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getfinero-com/openapi/getfinero-com-payments-api-openapi.yml
- filename: getfinero-com-scheduler-api-openapi.yml
  format: yaml
  label: Finero Scheduler API
  slug: getfinero-com-scheduler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getfinero-com/openapi/getfinero-com-scheduler-api-openapi.yml
- filename: getfinero-com-tasks-api-openapi.yml
  format: yaml
  label: Finero Tasks API
  slug: getfinero-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getfinero-com/openapi/getfinero-com-tasks-api-openapi.yml
- filename: getfinero-com-workflows-api-openapi.yml
  format: yaml
  label: Finero Workflows API
  slug: getfinero-com-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getfinero-com/openapi/getfinero-com-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Finero Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finero secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Finero
provider_slug: getfinero-com
scheme_count: 1
schemes:
- description: 'A Finero API key (`fnr_…`), created by a tenant admin in Settings → API. Sent as `Authorization: Bearer fnr_…`. Never place keys in URLs.'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/getfinero-com-openapi.json
  type: http
slug: getfinero-com-authentication
source_filename: getfinero-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/getfinero-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'A Finero API key (`fnr_…`), created by a tenant admin in Settings → API. Sent\n    as `Authorization: Bearer fnr_…`. Never place keys in URLs.'\n  sources:\n  - openapi/getfinero-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/getfinero-com/authentication/getfinero-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Fintech
- B2B
- Payments
- Automation
- ERP
---
