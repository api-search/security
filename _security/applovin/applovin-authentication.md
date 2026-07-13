---
api_key_in:
- header
- query
api_specs:
- filename: applovin-max-revenue-reporting.yaml
  format: yaml
  label: AppLovin MAX Revenue Reporting API
  slug: applovin-max-revenue-reporting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-max-revenue-reporting.yaml
- filename: applovin-max-ad-unit-management.yaml
  format: yaml
  label: AppLovin MAX Ad Unit Management API
  slug: applovin-max-ad-unit-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-max-ad-unit-management.yaml
- filename: applovin-growth-reporting.yaml
  format: yaml
  label: AppLovin Growth (Axon / AppDiscovery) Reporting API
  slug: applovin-growth-reporting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-growth-reporting.yaml
- filename: applovin-growth-asset-reporting.yaml
  format: yaml
  label: AppLovin Growth Asset Reporting API
  slug: applovin-growth-asset-reporting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-growth-asset-reporting.yaml
- filename: applovin-axon-campaign-management.yaml
  format: yaml
  label: AppLovin Axon Campaign Management API
  slug: applovin-axon-campaign-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-axon-campaign-management.yaml
- filename: applovin-conversion-api-lead-gen.yaml
  format: yaml
  label: AppLovin Conversion API for Lead Generation
  slug: applovin-conversion-api-lead-gen
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-conversion-api-lead-gen.yaml
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
