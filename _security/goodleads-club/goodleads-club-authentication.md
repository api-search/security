---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: goodleads-club-account-api-openapi.yml
  format: yaml
  label: GoodLeads Account API
  slug: goodleads-club-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-account-api-openapi.yml
- filename: goodleads-club-admin-api-openapi.yml
  format: yaml
  label: GoodLeads Admin API
  slug: goodleads-club-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-admin-api-openapi.yml
- filename: goodleads-club-agents-api-openapi.yml
  format: yaml
  label: GoodLeads Agents API
  slug: goodleads-club-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-agents-api-openapi.yml
- filename: goodleads-club-classification-api-openapi.yml
  format: yaml
  label: GoodLeads Classification API
  slug: goodleads-club-classification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-classification-api-openapi.yml
- filename: goodleads-club-commerce-api-openapi.yml
  format: yaml
  label: GoodLeads Commerce API
  slug: goodleads-club-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-commerce-api-openapi.yml
- filename: goodleads-club-concepts-api-openapi.yml
  format: yaml
  label: GoodLeads Concepts API
  slug: goodleads-club-concepts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-concepts-api-openapi.yml
- filename: goodleads-club-config-api-openapi.yml
  format: yaml
  label: GoodLeads Config API
  slug: goodleads-club-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-config-api-openapi.yml
- filename: goodleads-club-crm-api-openapi.yml
  format: yaml
  label: GoodLeads CRM API
  slug: goodleads-club-crm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-crm-api-openapi.yml
- filename: goodleads-club-enrichment-api-openapi.yml
  format: yaml
  label: GoodLeads Enrichment API
  slug: goodleads-club-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-enrichment-api-openapi.yml
- filename: goodleads-club-events-api-openapi.yml
  format: yaml
  label: GoodLeads Events API
  slug: goodleads-club-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-events-api-openapi.yml
- filename: goodleads-club-gm-api-openapi.yml
  format: yaml
  label: GoodLeads Gm API
  slug: goodleads-club-gm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-gm-api-openapi.yml
- filename: goodleads-club-health-api-openapi.yml
  format: yaml
  label: GoodLeads Health API
  slug: goodleads-club-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-health-api-openapi.yml
- filename: goodleads-club-leads-api-openapi.yml
  format: yaml
  label: GoodLeads Leads API
  slug: goodleads-club-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-leads-api-openapi.yml
- filename: goodleads-club-lists-api-openapi.yml
  format: yaml
  label: GoodLeads Lists API
  slug: goodleads-club-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-lists-api-openapi.yml
- filename: goodleads-club-monitoring-api-openapi.yml
  format: yaml
  label: GoodLeads Monitoring API
  slug: goodleads-club-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-monitoring-api-openapi.yml
- filename: goodleads-club-pipeline-api-openapi.yml
  format: yaml
  label: GoodLeads Pipeline API
  slug: goodleads-club-pipeline-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-pipeline-api-openapi.yml
- filename: goodleads-club-privacy-api-openapi.yml
  format: yaml
  label: GoodLeads Privacy API
  slug: goodleads-club-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-privacy-api-openapi.yml
- filename: goodleads-club-services-api-openapi.yml
  format: yaml
  label: GoodLeads Services API
  slug: goodleads-club-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-services-api-openapi.yml
- filename: goodleads-club-subscriptions-api-openapi.yml
  format: yaml
  label: GoodLeads Subscriptions API
  slug: goodleads-club-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-subscriptions-api-openapi.yml
- filename: goodleads-club-telemetry-api-openapi.yml
  format: yaml
  label: GoodLeads Telemetry API
  slug: goodleads-club-telemetry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goodleads-club/openapi/goodleads-club-telemetry-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: GoodLeads Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoodLeads secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GoodLeads
provider_slug: goodleads-club
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/goodleads-club-openapi.json
  type: apiKey
slug: goodleads-club-authentication
source_filename: goodleads-club-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/goodleads-club-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/goodleads-club-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/goodleads-club/authentication/goodleads-club-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- B2B
- Lead-Data
- Sales Enablement
---
