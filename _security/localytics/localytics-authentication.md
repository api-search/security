---
api_key_in:
- query
api_specs:
- filename: localytics-audiences-api-openapi.yml
  format: yaml
  label: Localytics Audiences API
  slug: localytics-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localytics/refs/heads/main/openapi/localytics-audiences-api-openapi.yml
- filename: localytics-campaigns-api-openapi.yml
  format: yaml
  label: Localytics Campaigns API
  slug: localytics-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localytics/refs/heads/main/openapi/localytics-campaigns-api-openapi.yml
- filename: localytics-push-campaigns-api-openapi.yml
  format: yaml
  label: Localytics Push Campaigns API
  slug: localytics-push-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localytics/refs/heads/main/openapi/localytics-push-campaigns-api-openapi.yml
- filename: localytics-meta-api-openapi.yml
  format: yaml
  label: Localytics Meta API
  slug: localytics-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localytics/refs/heads/main/openapi/localytics-meta-api-openapi.yml
- filename: localytics-push-api-openapi.yml
  format: yaml
  label: Localytics Push API
  slug: localytics-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/localytics/refs/heads/main/openapi/localytics-push-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Localytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Localytics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Localytics
provider_slug: localytics
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/localytics-audiences-api-openapi.yml
  - openapi/localytics-campaigns-api-openapi.yml
  - openapi/localytics-push-campaigns-api-openapi.yml
  type: http
slug: localytics-authentication
source_filename: localytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/localytics-audiences-api-openapi.yml, openapi/localytics-campaigns-api-openapi.yml,\n  openapi/localytics-push-campaigns-api-openapi.yml\nsummary:\n  types:\n  - http\n  http_schemes: [basic]\n  api_key_in: [query]\n  oauth2_flows: []\n  scopes: 0\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/localytics-audiences-api-openapi.yml\n  - openapi/localytics-campaigns-api-openapi.yml\n  - openapi/localytics-push-campaigns-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localytics/refs/heads/main/authentication/localytics-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Martech
- Mobile Analytics
- Push Notifications
- Customer Engagement
- Marketing Automation
- Mobile
- Segmentation
- Audiences
- Event Ingestion
- gRPC
---
