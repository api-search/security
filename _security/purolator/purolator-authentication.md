---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Purolator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Purolator secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Purolator
provider_slug: purolator
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: 'For secure access, this API uses Bearer Authentication (also known as token authentication). You must send a Bearer token in the Authorization header when making requests to protected endpoints. The token should be prefixed with the word "Bearer" followed by a space. Example: "Authorization: Bearer <YourTokenHere>".'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/purolator-close-manifest-openapi.yml
  - openapi/purolator-create-void-shipment-openapi.yml
  - openapi/purolator-estimate-openapi.yml
  - openapi/purolator-get-documents-openapi.yml
  - openapi/purolator-get-summary-manifest-openapi.yml
  - openapi/purolator-locator-openapi.yml
  - openapi/purolator-pickup-openapi.yml
  - openapi/purolator-tracking-openapi.yml
  type: http
- description: 'This API uses HTTP Basic Authentication to obtain a Bearer token. Provide your `client_id` as

    the username and `client_secret` as the password, Base64-encoded in the `Authorization` header.

    Example: "Authorization: Basic <base64(client_id:client_secret)>"'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/purolator-token-openapi.yml
  type: http
- description: "For authenticating requests using AWS Signature Version 4. The value of this header must be \nformed according to AWS Signature Version 4 specifications. This includes the algorithm \nidentifier (AWS4-HMAC-SHA256), followed by credential scope, a list of signed headers, and \nthe signature. Refer to AWS documentation for detailed instructions on forming this header."
  in: header
  name: AWSv4Auth
  parameter: Authorization
  sources:
  - openapi/purolator-token-openapi.yml
  type: apiKey
slug: purolator-authentication
source_filename: purolator-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/purolator-close-manifest-openapi.yml, openapi/purolator-create-void-shipment-openapi.yml,\n  openapi/purolator-estimate-openapi.yml, openapi/purolator-get-documents-openapi.yml, openapi/purolator-get-summary-manifest-openapi.yml,\n  openapi/purolator-locator-openapi.yml, openapi/purolator-pickup-openapi.yml, openapi/purolator-token-openapi.yml,\n  openapi/purolator-tracking-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'For secure access, this API uses Bearer Authentication (also known as token\n    authentication). You must send a Bearer token in the Authorization header when making requests\n    to protected endpoints. The token should be prefixed with the word \"Bearer\" followed by\n    a space. Example: \"Authorization: Bearer <YourTokenHere>\".'\n  sources:\n  - openapi/purolator-close-manifest-openapi.yml\n\
  \  - openapi/purolator-create-void-shipment-openapi.yml\n  - openapi/purolator-estimate-openapi.yml\n  - openapi/purolator-get-documents-openapi.yml\n  - openapi/purolator-get-summary-manifest-openapi.yml\n  - openapi/purolator-locator-openapi.yml\n  - openapi/purolator-pickup-openapi.yml\n  - openapi/purolator-tracking-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    This API uses HTTP Basic Authentication to obtain a Bearer token. Provide your `client_id` as\n    the username and `client_secret` as the password, Base64-encoded in the `Authorization` header.\n    Example: \"Authorization: Basic <base64(client_id:client_secret)>\"\n  sources:\n  - openapi/purolator-token-openapi.yml\n- name: AWSv4Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: \"For authenticating requests using AWS Signature Version 4. The value of this\\\n    \\ header must be \\nformed according to AWS Signature Version 4 specifications. This includes\\\
  \n    \\ the algorithm \\nidentifier (AWS4-HMAC-SHA256), followed by credential scope, a list of\\\n    \\ signed headers, and \\nthe signature. Refer to AWS documentation for detailed instructions\\\n    \\ on forming this header.\"\n  sources:\n  - openapi/purolator-token-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/purolator/authentication/purolator-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Shipping
- Logistics
- Couriers
- Freight
---
