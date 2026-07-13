---
api_key_in: []
api_specs:
- filename: 1nce-authorization-openapi.yml
  format: yaml
  label: 1NCE Authorization API
  slug: 1nce-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1nce/refs/heads/main/openapi/1nce-authorization-openapi.yml
- filename: 1nce-sim-management-openapi.yml
  format: yaml
  label: 1NCE SIM Management API
  slug: 1nce-sim-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1nce/refs/heads/main/openapi/1nce-sim-management-openapi.yml
- filename: 1nce-os-openapi.yml
  format: yaml
  label: 1NCE OS API
  slug: 1nce-os-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1nce/refs/heads/main/openapi/1nce-os-openapi.yml
- filename: 1nce-order-management-openapi.yml
  format: yaml
  label: 1NCE Order Management API
  slug: 1nce-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1nce/refs/heads/main/openapi/1nce-order-management-openapi.yml
- filename: 1nce-product-information-openapi.yml
  format: yaml
  label: 1NCE Product Information API
  slug: 1nce-product-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1nce/refs/heads/main/openapi/1nce-product-information-openapi.yml
- filename: 1nce-support-management-openapi.yml
  format: yaml
  label: 1NCE Support Management API
  slug: 1nce-support-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1nce/refs/heads/main/openapi/1nce-support-management-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: 1Nce Authentication
name_suffix: Authentication
oauth_flows: []
overview: 1NCE secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: 1NCE
provider_slug: 1nce
scheme_count: 2
schemes:
- description: Basic authentication used for obtaining the Bearer Authentication Token. The Bearer Token can then be used to make any further API calls towards the 1NCE API.
  name: BasicAuthentication
  scheme: basic
  sources:
  - openapi/1nce-authorization-openapi.yml
  - openapi/1nce-authorization-v2-openapi.yml
  type: http
- description: Bearer Authentication Token used to gain access to the 1NCE API. Please refer to the Open Authorization (/oauth/token) request for obtaining a Bearer Token.
  name: BearerAuthentication
  scheme: bearer
  sources:
  - openapi/1nce-order-management-openapi.yml
  - openapi/1nce-os-openapi.yml
  - openapi/1nce-product-information-openapi.yml
  - openapi/1nce-sim-management-openapi.yml
  - openapi/1nce-sim-management-v2-openapi.yml
  - openapi/1nce-support-management-openapi.yml
  type: http
slug: 1nce-authentication
source_filename: 1nce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/1nce-authorization-openapi.yml, openapi/1nce-authorization-v2-openapi.yml, openapi/1nce-order-management-openapi.yml,\n  openapi/1nce-os-openapi.yml, openapi/1nce-product-information-openapi.yml, openapi/1nce-sim-management-openapi.yml,\n  openapi/1nce-sim-management-v2-openapi.yml, openapi/1nce-support-management-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuthentication\n  type: http\n  scheme: basic\n  description: Basic authentication used for obtaining the Bearer Authentication Token. The\n    Bearer Token can then be used to make any further API calls towards the 1NCE API.\n  sources:\n  - openapi/1nce-authorization-openapi.yml\n  - openapi/1nce-authorization-v2-openapi.yml\n- name: BearerAuthentication\n  type: http\n  scheme: bearer\n  description: Bearer Authentication Token used to gain access to the 1NCE API. Please refer\n    to the Open Authorization (/oauth/token) request for obtaining\
  \ a Bearer Token.\n  sources:\n  - openapi/1nce-order-management-openapi.yml\n  - openapi/1nce-os-openapi.yml\n  - openapi/1nce-product-information-openapi.yml\n  - openapi/1nce-sim-management-openapi.yml\n  - openapi/1nce-sim-management-v2-openapi.yml\n  - openapi/1nce-support-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1nce/refs/heads/main/authentication/1nce-authentication.yml
summary_line: http · 2 schemes
tags:
- IoT
- Connectivity
- SIM
- Cellular
- NB-IoT
- LTE-M
- eUICC
- Edge
- Embedded
- Global Roaming
---
