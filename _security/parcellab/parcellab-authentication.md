---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: parcellab-events-api-openapi.yml
  format: yaml
  label: parcelLab Events API
  slug: parcellab-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-events-api-openapi.yml
- filename: parcellab-place-info-api-openapi.yml
  format: yaml
  label: parcelLab Place Info API
  slug: parcellab-place-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-place-info-api-openapi.yml
- filename: parcellab-promise-api-openapi.yml
  format: yaml
  label: parcelLab Promise API
  slug: parcellab-promise-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-promise-api-openapi.yml
- filename: parcellab-agents-api-openapi.yml
  format: yaml
  label: parcelLab Agents API
  slug: parcellab-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-agents-api-openapi.yml
- filename: parcellab-apps-api-openapi.yml
  format: yaml
  label: parcelLab Apps API
  slug: parcellab-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-apps-api-openapi.yml
- filename: parcellab-campaign-api-openapi.yml
  format: yaml
  label: parcelLab Campaign API
  slug: parcellab-campaign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-campaign-api-openapi.yml
- filename: parcellab-customer-portals-api-openapi.yml
  format: yaml
  label: parcelLab Customer Portals API
  slug: parcellab-customer-portals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-customer-portals-api-openapi.yml
- filename: parcellab-order-api-openapi.yml
  format: yaml
  label: parcelLab Order API
  slug: parcellab-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-order-api-openapi.yml
- filename: parcellab-order-status-page-theme-api-openapi.yml
  format: yaml
  label: parcelLab Order Status Page Theme API
  slug: parcellab-order-status-page-theme-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-order-status-page-theme-api-openapi.yml
- filename: parcellab-return-configuration-set-api-openapi.yml
  format: yaml
  label: parcelLab Return Configuration Set API
  slug: parcellab-return-configuration-set-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-return-configuration-set-api-openapi.yml
- filename: parcellab-return-registration-api-openapi.yml
  format: yaml
  label: parcelLab Return Registration API
  slug: parcellab-return-registration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-return-registration-api-openapi.yml
- filename: parcellab-size-recommender-api-openapi.yml
  format: yaml
  label: parcelLab Size Recommender API
  slug: parcellab-size-recommender-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-size-recommender-api-openapi.yml
- filename: parcellab-survey-api-openapi.yml
  format: yaml
  label: parcelLab Survey API
  slug: parcellab-survey-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-survey-api-openapi.yml
- filename: parcellab-theme-api-openapi.yml
  format: yaml
  label: parcelLab Theme API
  slug: parcellab-theme-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-theme-api-openapi.yml
- filename: parcellab-translation-api-openapi.yml
  format: yaml
  label: parcelLab Translation API
  slug: parcellab-translation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-translation-api-openapi.yml
- filename: parcellab-voucher-api-openapi.yml
  format: yaml
  label: parcelLab Voucher API
  slug: parcellab-voucher-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parcellab/openapi/parcellab-voucher-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: parcelLab Authentication
name_suffix: Authentication
oauth_flows: []
overview: parcelLab secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: parcelLab
provider_slug: parcellab
scheme_count: 1
schemes:
- description: '`Authorization: Parcellab-API-Token <base64(account_id:token)>`. App- generated tokens may instead use the `Bearer <token>` scheme.'
  in: header
  name: parcellabApiToken
  parameter: Authorization
  sources:
  - openapi/parcellab-openapi.yml
  type: apiKey
slug: parcellab-authentication
source_filename: parcellab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/parcellab-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: parcellabApiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: '`Authorization: Parcellab-API-Token <base64(account_id:token)>`. App- generated\n    tokens may instead use the `Bearer <token>` scheme.'\n  sources:\n  - openapi/parcellab-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/parcellab/authentication/parcellab-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Post-Purchase
- E-Commerce
- Tracking
- Returns
- Shipping
- Delivery
- Customer Experience
- Logistics
- Communications
- Germany
---
