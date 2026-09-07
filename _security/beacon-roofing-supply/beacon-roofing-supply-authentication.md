---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: beacon-roofing-supply-v2-openapi.yml
  format: yaml
  label: Beacon PRO+ API (V2, OAuth)
  slug: beacon-pro-plus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-v2-openapi.yml
- filename: beacon-roofing-supply-all-api-openapi.yml
  format: yaml
  label: Beacon External Rest Service (all_api)
  slug: beacon-rest-all-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-all-api-openapi.yml
- filename: beacon-roofing-supply-v3-openapi.yml
  format: yaml
  label: Beacon Rest Services V3 (Public / Integrations)
  slug: beacon-rest-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-v3-openapi.yml
- filename: beacon-roofing-supply-v1-openapi.yml
  format: yaml
  label: Beacon Rest Services V1 (session)
  slug: beacon-rest-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-v1-openapi.yml
- filename: beacon-roofing-supply-oauth2-openapi.yml
  format: yaml
  label: Beacon OAuth Rest Service
  slug: beacon-oauth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-oauth2-openapi.yml
- filename: beacon-roofing-supply-public-openapi.yml
  format: yaml
  label: Beacon Rest Services Public
  slug: beacon-rest-public
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-public-openapi.yml
- filename: beacon-roofing-supply-internal-openapi.yml
  format: yaml
  label: Beacon Internal Rest Service
  slug: beacon-rest-internal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-internal-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: derived
name: Beacon Roofing Supply Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beacon Roofing Supply secures its APIs with apiKey and http across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Beacon Roofing Supply
provider_slug: beacon-roofing-supply
scheme_count: 6
schemes:
- bearerFormat: token
  name: internalAuth
  scheme: bearer
  sources:
  - openapi/beacon-roofing-supply-internal-ng-openapi.yml
  - openapi/beacon-roofing-supply-internal-openapi.yml
  - openapi/beacon-roofing-supply-public-openapi.yml
  - openapi/beacon-roofing-supply-v3-ng-openapi.yml
  - openapi/beacon-roofing-supply-v3-openapi.yml
  type: http
- in: cookie
  name: JSESSIONID
  parameter: JSESSIONID
  sources:
  - openapi/beacon-roofing-supply-v1-ng-openapi.yml
  - openapi/beacon-roofing-supply-v1-openapi.yml
  - openapi/beacon-roofing-supply-v2-ng-openapi.yml
  - openapi/beacon-roofing-supply-v2-openapi.yml
  type: apiKey
- in: cookie
  name: DYN_USER_ID
  parameter: DYN_USER_ID
  sources:
  - openapi/beacon-roofing-supply-v1-ng-openapi.yml
  - openapi/beacon-roofing-supply-v1-openapi.yml
  - openapi/beacon-roofing-supply-v2-ng-openapi.yml
  - openapi/beacon-roofing-supply-v2-openapi.yml
  type: apiKey
- in: cookie
  name: DYN_USER_CONFIRM
  parameter: DYN_USER_CONFIRM
  sources:
  - openapi/beacon-roofing-supply-v1-ng-openapi.yml
  - openapi/beacon-roofing-supply-v1-openapi.yml
  - openapi/beacon-roofing-supply-v2-ng-openapi.yml
  - openapi/beacon-roofing-supply-v2-openapi.yml
  type: apiKey
- in: cookie
  name: siteId
  parameter: siteId
  sources:
  - openapi/beacon-roofing-supply-v1-ng-openapi.yml
  - openapi/beacon-roofing-supply-v1-openapi.yml
  - openapi/beacon-roofing-supply-v2-ng-openapi.yml
  - openapi/beacon-roofing-supply-v2-openapi.yml
  type: apiKey
- in: cookie
  name: rememberPassword
  parameter: rememberPassword
  sources:
  - openapi/beacon-roofing-supply-v1-ng-openapi.yml
  - openapi/beacon-roofing-supply-v1-openapi.yml
  type: apiKey
slug: beacon-roofing-supply-authentication
source_filename: beacon-roofing-supply-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: derived\nsource: openapi/beacon-roofing-supply-internal-ng-openapi.yml, openapi/beacon-roofing-supply-internal-openapi.yml,\n  openapi/beacon-roofing-supply-public-openapi.yml, openapi/beacon-roofing-supply-v1-ng-openapi.yml,\n  openapi/beacon-roofing-supply-v1-openapi.yml, openapi/beacon-roofing-supply-v2-ng-openapi.yml,\n  openapi/beacon-roofing-supply-v2-openapi.yml, openapi/beacon-roofing-supply-v3-ng-openapi.yml,\n  openapi/beacon-roofing-supply-v3-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: internalAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  sources:\n  - openapi/beacon-roofing-supply-internal-ng-openapi.yml\n  - openapi/beacon-roofing-supply-internal-openapi.yml\n  - openapi/beacon-roofing-supply-public-openapi.yml\n  - openapi/beacon-roofing-supply-v3-ng-openapi.yml\n  - openapi/beacon-roofing-supply-v3-openapi.yml\n- name: JSESSIONID\n  type: apiKey\n  in: cookie\n\
  \  parameter: JSESSIONID\n  sources:\n  - openapi/beacon-roofing-supply-v1-ng-openapi.yml\n  - openapi/beacon-roofing-supply-v1-openapi.yml\n  - openapi/beacon-roofing-supply-v2-ng-openapi.yml\n  - openapi/beacon-roofing-supply-v2-openapi.yml\n- name: DYN_USER_ID\n  type: apiKey\n  in: cookie\n  parameter: DYN_USER_ID\n  sources:\n  - openapi/beacon-roofing-supply-v1-ng-openapi.yml\n  - openapi/beacon-roofing-supply-v1-openapi.yml\n  - openapi/beacon-roofing-supply-v2-ng-openapi.yml\n  - openapi/beacon-roofing-supply-v2-openapi.yml\n- name: DYN_USER_CONFIRM\n  type: apiKey\n  in: cookie\n  parameter: DYN_USER_CONFIRM\n  sources:\n  - openapi/beacon-roofing-supply-v1-ng-openapi.yml\n  - openapi/beacon-roofing-supply-v1-openapi.yml\n  - openapi/beacon-roofing-supply-v2-ng-openapi.yml\n  - openapi/beacon-roofing-supply-v2-openapi.yml\n- name: siteId\n  type: apiKey\n  in: cookie\n  parameter: siteId\n  sources:\n  - openapi/beacon-roofing-supply-v1-ng-openapi.yml\n  - openapi/beacon-roofing-supply-v1-openapi.yml\n\
  \  - openapi/beacon-roofing-supply-v2-ng-openapi.yml\n  - openapi/beacon-roofing-supply-v2-openapi.yml\n- name: rememberPassword\n  type: apiKey\n  in: cookie\n  parameter: rememberPassword\n  sources:\n  - openapi/beacon-roofing-supply-v1-ng-openapi.yml\n  - openapi/beacon-roofing-supply-v1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/authentication/beacon-roofing-supply-authentication.yml
summary_line: apiKey/http · 6 schemes
tags:
- Construction
- Distribution
- Roofing
- Building Materials
- E-Commerce
- Fortune 1000
- Supply Chain
- Order
- Catalog
- Delivery
---
