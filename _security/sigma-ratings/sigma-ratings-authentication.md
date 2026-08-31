---
api_key_in:
- header
api_specs:
- filename: sigma-ratings-account-api-openapi.yml
  format: yaml
  label: Sigma360 Account API
  slug: sigma-ratings-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sigma-ratings/refs/heads/main/openapi/sigma-ratings-account-api-openapi.yml
- filename: sigma-ratings-informational-api-openapi.yml
  format: yaml
  label: Sigma360 Informational API
  slug: sigma-ratings-informational-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sigma-ratings/refs/heads/main/openapi/sigma-ratings-informational-api-openapi.yml
- filename: sigma-ratings-monitoring-entity-creation-api-openapi.yml
  format: yaml
  label: 'Sigma360 Monitoring: Entity Creation API'
  slug: sigma-ratings-monitoring-entity-creation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sigma-ratings/refs/heads/main/openapi/sigma-ratings-monitoring-entity-creation-api-openapi.yml
- filename: sigma-ratings-monitoring-entity-management-api-openapi.yml
  format: yaml
  label: 'Sigma360 Monitoring: Entity Management API'
  slug: sigma-ratings-monitoring-entity-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sigma-ratings/refs/heads/main/openapi/sigma-ratings-monitoring-entity-management-api-openapi.yml
- filename: sigma-ratings-monitoring-history-api-openapi.yml
  format: yaml
  label: 'Sigma360 Monitoring: History API'
  slug: sigma-ratings-monitoring-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sigma-ratings/refs/heads/main/openapi/sigma-ratings-monitoring-history-api-openapi.yml
- filename: sigma-ratings-one-off-screening-api-openapi.yml
  format: yaml
  label: Sigma360 One-Off Screening API
  slug: sigma-ratings-one-off-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sigma-ratings/refs/heads/main/openapi/sigma-ratings-one-off-screening-api-openapi.yml
- filename: sigma-ratings-utilities-api-openapi.yml
  format: yaml
  label: Sigma360 Utilities API
  slug: sigma-ratings-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sigma-ratings/refs/heads/main/openapi/sigma-ratings-utilities-api-openapi.yml
- filename: sigma-ratings-webhooks-api-openapi.yml
  format: yaml
  label: Sigma360 Webhooks API
  slug: sigma-ratings-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sigma-ratings/refs/heads/main/openapi/sigma-ratings-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sigma Ratings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sigma360 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sigma360
provider_slug: sigma-ratings
scheme_count: 1
schemes:
- description: API Key
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/sigma-ratings-openapi-original.json
  type: apiKey
slug: sigma-ratings-authentication
source_filename: sigma-ratings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sigma-ratings-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API Key\n  sources:\n  - openapi/sigma-ratings-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sigma-ratings/refs/heads/main/authentication/sigma-ratings-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Compliance
- Financial Crime
- KYC
- AML
- Sanctions Screening
- Risk Intelligence
- RegTech
- Adverse Media
---
