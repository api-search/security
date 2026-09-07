---
anonymous_access: false
api_key_in: []
api_specs:
- filename: diebold-dn-open-backend-api-openapi.yml
  format: yaml
  label: DN Open Backend API
  slug: dn-open-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-dn-open-backend-api-openapi.yml
- filename: diebold-dn-online-mobile-api-openapi.yml
  format: yaml
  label: DN Online & Mobile API
  slug: dn-online-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-dn-online-mobile-api-openapi.yml
- filename: diebold-dn-assist-api-openapi.yml
  format: yaml
  label: DN Assist API
  slug: dn-assist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-dn-assist-api-openapi.yml
- filename: diebold-dn-payment-initiation-api-openapi.yml
  format: yaml
  label: DN Payment Initiation API
  slug: dn-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-dn-payment-initiation-api-openapi.yml
- filename: diebold-dn-tm-authorization-api-openapi.yml
  format: yaml
  label: DN TM Authorization API
  slug: dn-tm-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-dn-tm-authorization-api-openapi.yml
- filename: diebold-dn-account-bc-api-openapi.yml
  format: yaml
  label: DN Account BC API
  slug: dn-account-bc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-dn-account-bc-api-openapi.yml
- filename: diebold-dn-secure-business-processing-api-openapi.yml
  format: yaml
  label: DN Secure Business Processing API
  slug: dn-secure-business-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-dn-secure-business-processing-api-openapi.yml
- filename: diebold-tm-pre-digitization-api-outbound-openapi.yml
  format: yaml
  label: TM Pre-Digitization API (Outbound)
  slug: tm-pre-digitization-api-outbound
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-tm-pre-digitization-api-outbound-openapi.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Diebold Authentication
name_suffix: Authentication
oauth_flows: []
overview: Diebold Nixdorf secures its APIs with http and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Diebold Nixdorf
provider_slug: diebold
scheme_count: 3
schemes:
- description: Authorization will contain base 64 encoded userName:password string
  name: basic
  scheme: basic
  sources:
  - openapi/diebold-dn-assist-api-openapi.yml
  - openapi/diebold-dn-open-backend-api-openapi.yml
  - openapi/diebold-dn-secure-business-processing-api-openapi.yml
  - openapi/diebold-dn-tm-authorization-api-openapi.yml
  type: http
- bearerFormat: Any string
  description: Authorization will contain token received using getToken request as Bearer Token
  name: bearer
  scheme: bearer
  sources:
  - openapi/diebold-dn-assist-api-openapi.yml
  - openapi/diebold-dn-online-mobile-api-openapi.yml
  - openapi/diebold-dn-open-backend-api-openapi.yml
  - openapi/diebold-dn-payment-initiation-api-openapi.yml
  - openapi/diebold-dn-tm-authorization-api-openapi.yml
  type: http
- name: openId
  openIdConnectUrl: https://login.microsoftonline.com/52846f0f-bc96-4a36-939b-f4d04bb473a0/v2.0/.well-known/openid-configuration
  sources:
  - openapi/diebold-dn-payment-initiation-api-openapi.yml
  type: openIdConnect
slug: diebold-authentication
source_filename: diebold-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: derived\nsource: openapi/diebold-dn-assist-api-openapi.yml, openapi/diebold-dn-online-mobile-api-openapi.yml,\n  openapi/diebold-dn-open-backend-api-openapi.yml, openapi/diebold-dn-payment-initiation-api-openapi.yml,\n  openapi/diebold-dn-secure-business-processing-api-openapi.yml, openapi/diebold-dn-tm-authorization-api-openapi.yml\nsummary:\n  types:\n  - http\n  - openIdConnect\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  description: Authorization will contain base 64 encoded userName:password string\n  sources:\n  - openapi/diebold-dn-assist-api-openapi.yml\n  - openapi/diebold-dn-open-backend-api-openapi.yml\n  - openapi/diebold-dn-secure-business-processing-api-openapi.yml\n  - openapi/diebold-dn-tm-authorization-api-openapi.yml\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: Any string\n  description: Authorization will contain token received using getToken request as Bearer Token\n  sources:\n  - openapi/diebold-dn-assist-api-openapi.yml\n\
  \  - openapi/diebold-dn-online-mobile-api-openapi.yml\n  - openapi/diebold-dn-open-backend-api-openapi.yml\n  - openapi/diebold-dn-payment-initiation-api-openapi.yml\n  - openapi/diebold-dn-tm-authorization-api-openapi.yml\n- name: openId\n  type: openIdConnect\n  openIdConnectUrl: https://login.microsoftonline.com/52846f0f-bc96-4a36-939b-f4d04bb473a0/v2.0/.well-known/openid-configuration\n  sources:\n  - openapi/diebold-dn-payment-initiation-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/authentication/diebold-authentication.yml
summary_line: http/openIdConnect · 3 schemes
tags:
- Banking
- Retail
- ATM
- Self-Service
- Point-of-Sale
- Payments
- Transaction Middleware
- Vynamic
- Open Banking
- Fortune 1000
---
