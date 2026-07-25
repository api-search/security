---
api_key_in:
- header
- query
api_specs:
- filename: applovin-ad-units-api-openapi.yml
  format: yaml
  label: AppLovin Ad Units API
  slug: applovin-ad-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-ad-units-api-openapi.yml
- filename: applovin-asset-reporting-api-openapi.yml
  format: yaml
  label: AppLovin Asset Reporting API
  slug: applovin-asset-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-asset-reporting-api-openapi.yml
- filename: applovin-assets-api-openapi.yml
  format: yaml
  label: AppLovin Assets API
  slug: applovin-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-assets-api-openapi.yml
- filename: applovin-campaigns-api-openapi.yml
  format: yaml
  label: AppLovin Campaigns API
  slug: applovin-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-campaigns-api-openapi.yml
- filename: applovin-conversion-events-api-openapi.yml
  format: yaml
  label: AppLovin Conversion Events API
  slug: applovin-conversion-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-conversion-events-api-openapi.yml
- filename: applovin-creative-sets-api-openapi.yml
  format: yaml
  label: AppLovin Creative Sets API
  slug: applovin-creative-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-creative-sets-api-openapi.yml
- filename: applovin-experiments-api-openapi.yml
  format: yaml
  label: AppLovin Experiments API
  slug: applovin-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-experiments-api-openapi.yml
- filename: applovin-growth-reporting-api-openapi.yml
  format: yaml
  label: AppLovin Growth Reporting API
  slug: applovin-growth-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-growth-reporting-api-openapi.yml
- filename: applovin-revenue-reporting-api-openapi.yml
  format: yaml
  label: AppLovin Revenue Reporting API
  slug: applovin-revenue-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-revenue-reporting-api-openapi.yml
- filename: applovin-test-devices-api-openapi.yml
  format: yaml
  label: AppLovin Test Devices API
  slug: applovin-test-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-test-devices-api-openapi.yml
- filename: applovin-waterfalls-api-openapi.yml
  format: yaml
  label: AppLovin Waterfalls API
  slug: applovin-waterfalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-waterfalls-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Applovin Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppLovin secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AppLovin
provider_slug: applovin
scheme_count: 3
schemes:
- description: Campaign Management API key passed in the `Authorization` header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/applovin-axon-campaign-management.yaml
  - openapi/applovin-conversion-api-lead-gen.yaml
  type: http
- in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/applovin-growth-asset-reporting.yaml
  - openapi/applovin-growth-reporting.yaml
  - openapi/applovin-max-revenue-reporting.yaml
  type: apiKey
- description: Management Key from AppLovin dashboard (Account > General > Keys).
  in: header
  name: apiKeyHeader
  parameter: Api-Key
  sources:
  - openapi/applovin-max-ad-unit-management.yaml
  type: apiKey
slug: applovin-authentication
source_filename: applovin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/applovin-axon-campaign-management.yaml, openapi/applovin-conversion-api-lead-gen.yaml,\n  openapi/applovin-growth-asset-reporting.yaml, openapi/applovin-growth-reporting.yaml, openapi/applovin-max-ad-unit-management.yaml,\n  openapi/applovin-max-revenue-reporting.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Campaign Management API key passed in the `Authorization` header.\n  sources:\n  - openapi/applovin-axon-campaign-management.yaml\n  - openapi/applovin-conversion-api-lead-gen.yaml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/applovin-growth-asset-reporting.yaml\n  - openapi/applovin-growth-reporting.yaml\n  - openapi/applovin-max-revenue-reporting.yaml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: Management\
  \ Key from AppLovin dashboard (Account > General > Keys).\n  sources:\n  - openapi/applovin-max-ad-unit-management.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/authentication/applovin-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Advertising
- Mobile
- AdTech
- App Monetization
- Mediation
- User Acquisition
- Marketing Technology
- Conversion Tracking
---
