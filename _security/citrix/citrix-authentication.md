---
api_key_in:
- cookie
- header
api_specs:
- filename: openapi
  format: yaml
  label: Citrix Virtual Apps and Desktops REST API
  slug: citrix-virtual-apps-and-desktops-rest-api
  spec_type: OpenAPI
  url: https://developer.citrix.com/citrix-virtual-apps-and-desktops/citrix-cvad-rest-apis/docs/openapi
- filename: citrix-adc-nitro-openapi.yml
  format: yaml
  label: Citrix ADC (NetScaler) NITRO API
  slug: citrix-adc-netscaler-nitro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix/refs/heads/main/openapi/citrix-adc-nitro-openapi.yml
- filename: openapi
  format: yaml
  label: Citrix DaaS REST API
  slug: citrix-daas-rest-api
  spec_type: OpenAPI
  url: https://developer.citrix.com/citrix-daas/citrix-daas-rest-apis/docs/openapi
- filename: citrix-cloud-openapi.yml
  format: yaml
  label: Citrix Cloud API
  slug: citrix-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix/refs/heads/main/openapi/citrix-cloud-openapi.yml
- filename: citrix-storefront-web-openapi.yml
  format: yaml
  label: Citrix StoreFront Web API
  slug: citrix-storefront-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix/refs/heads/main/openapi/citrix-storefront-web-openapi.yml
- filename: citrix-endpoint-management-openapi.yml
  format: yaml
  label: Citrix Endpoint Management REST API
  slug: citrix-endpoint-management-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix/refs/heads/main/openapi/citrix-endpoint-management-openapi.yml
- filename: citrix-secure-private-access-openapi.yml
  format: yaml
  label: Citrix Secure Private Access API
  slug: citrix-secure-private-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix/refs/heads/main/openapi/citrix-secure-private-access-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Citrix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Citrix secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Citrix
provider_slug: citrix
scheme_count: 4
schemes:
- description: Session cookie from NITRO login
  in: cookie
  name: nitroAuth
  parameter: NITRO_AUTH_TOKEN
  sources:
  - openapi/citrix-adc-nitro-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: OAuth 2.0 bearer token from client credentials grant
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/citrix-cloud-openapi.yml
  - openapi/citrix-daas-openapi.yml
  - openapi/citrix-secure-private-access-openapi.yml
  type: http
- description: Authentication token from login endpoint
  in: header
  name: authToken
  parameter: auth_token
  sources:
  - openapi/citrix-endpoint-management-openapi.yml
  type: apiKey
- description: CSRF token from session cookie for POST requests
  in: header
  name: csrfToken
  parameter: Csrf-Token
  sources:
  - openapi/citrix-storefront-web-openapi.yml
  type: apiKey
slug: citrix-authentication
source_filename: citrix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/citrix-adc-nitro-openapi.yml, openapi/citrix-cloud-openapi.yml, openapi/citrix-daas-openapi.yml,\n  openapi/citrix-endpoint-management-openapi.yml, openapi/citrix-secure-private-access-openapi.yml,\n  openapi/citrix-storefront-web-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: nitroAuth\n  type: apiKey\n  in: cookie\n  parameter: NITRO_AUTH_TOKEN\n  description: Session cookie from NITRO login\n  sources:\n  - openapi/citrix-adc-nitro-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token from client credentials grant\n  sources:\n  - openapi/citrix-cloud-openapi.yml\n  - openapi/citrix-daas-openapi.yml\n  - openapi/citrix-secure-private-access-openapi.yml\n- name: authToken\n  type: apiKey\n  in: header\n  parameter: auth_token\n  description: Authentication token from login endpoint\n\
  \  sources:\n  - openapi/citrix-endpoint-management-openapi.yml\n- name: csrfToken\n  type: apiKey\n  in: header\n  parameter: Csrf-Token\n  description: CSRF token from session cookie for POST requests\n  sources:\n  - openapi/citrix-storefront-web-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citrix/refs/heads/main/authentication/citrix-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Application Delivery
- Desktop-As-A-Service
- Networking
- Virtualization
- Workspace
- Fortune 1000
---
