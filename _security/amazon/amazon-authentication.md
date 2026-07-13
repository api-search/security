---
api_key_in:
- header
api_specs:
- filename: amazon-selling-partner-api-openapi.yml
  format: yaml
  label: Amazon Selling Partner API
  slug: selling-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-selling-partner-api-openapi.yml
- filename: amazon-advertising-api-openapi.yml
  format: yaml
  label: Amazon Advertising API
  slug: advertising-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-advertising-api-openapi.yml
- filename: amazon-pay-api-openapi.yml
  format: yaml
  label: Amazon Pay API
  slug: pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-pay-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Amazon
provider_slug: amazon
scheme_count: 2
schemes:
- description: OAuth 2.0 access token from Login with Amazon
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/amazon-advertising-api-openapi.yml
  - openapi/amazon-selling-partner-api-openapi.yml
  type: http
- description: AMZN-PAY-RSASSA-PSS-V2 signature using merchant private key
  in: header
  name: amazonPaySignature
  parameter: authorization
  sources:
  - openapi/amazon-pay-api-openapi.yml
  type: apiKey
slug: amazon-authentication
source_filename: amazon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-advertising-api-openapi.yml, openapi/amazon-pay-api-openapi.yml, openapi/amazon-selling-partner-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token from Login with Amazon\n  sources:\n  - openapi/amazon-advertising-api-openapi.yml\n  - openapi/amazon-selling-partner-api-openapi.yml\n- name: amazonPaySignature\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: AMZN-PAY-RSASSA-PSS-V2 signature using merchant private key\n  sources:\n  - openapi/amazon-pay-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/authentication/amazon-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
- Fortune 100
---
