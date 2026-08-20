---
api_key_in:
- header
api_specs:
- filename: moloco-ads-campaign-management-openapi.yml
  format: yaml
  label: Moloco Ads Campaign Management API
  slug: moloco-ads-campaign-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-ads-campaign-management-openapi.yml
- filename: moloco-cloud-auth-openapi.yml
  format: yaml
  label: Moloco Cloud Auth API
  slug: moloco-cloud-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-cloud-auth-openapi.yml
- filename: moloco-commerce-media-management-openapi.yml
  format: yaml
  label: Moloco Commerce Media Management API
  slug: moloco-commerce-media-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-commerce-media-management-openapi.yml
- filename: moloco-commerce-media-decision-openapi.yml
  format: yaml
  label: Moloco Commerce Media Decision API
  slug: moloco-commerce-media-decision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-commerce-media-decision-openapi.yml
- filename: moloco-commerce-media-event-openapi.yml
  format: yaml
  label: Moloco Commerce Media Event API
  slug: moloco-commerce-media-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-commerce-media-event-openapi.yml
- filename: moloco-commerce-media-webhooks-openapi.yml
  format: yaml
  label: Moloco Commerce Media Webhooks
  slug: moloco-commerce-media-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-commerce-media-webhooks-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Moloco Authentication
name_suffix: Authentication
oauth_flows: []
overview: MOLOCO secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MOLOCO
provider_slug: moloco
scheme_count: 2
schemes:
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/moloco-ads-campaign-management-openapi.yml
  - openapi/moloco-cloud-auth-openapi.yml
  - openapi/moloco-commerce-media-management-openapi.yml
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/moloco-commerce-media-decision-openapi.yml
  - openapi/moloco-commerce-media-event-openapi.yml
  - openapi/moloco-commerce-media-management-openapi.yml
  type: apiKey
slug: moloco-authentication
source_filename: moloco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: derived\nsource: openapi/moloco-ads-campaign-management-openapi.yml, openapi/moloco-cloud-auth-openapi.yml,\n  openapi/moloco-commerce-media-decision-openapi.yml, openapi/moloco-commerce-media-event-openapi.yml,\n  openapi/moloco-commerce-media-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/moloco-ads-campaign-management-openapi.yml\n  - openapi/moloco-cloud-auth-openapi.yml\n  - openapi/moloco-commerce-media-management-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/moloco-commerce-media-decision-openapi.yml\n  - openapi/moloco-commerce-media-event-openapi.yml\n  - openapi/moloco-commerce-media-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/authentication/moloco-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Advertising
- AdTech
- Demand-Side Platform
- Retail Media
- Commerce Media
- Programmatic Advertising
- Campaign Management
- Ad Serving
- Machine-Learning
- Mobile Marketing
- Reporting
- user-events
---
