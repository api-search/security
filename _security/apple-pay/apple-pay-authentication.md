---
api_key_in: []
api_specs:
- filename: apple-pay-merchant-registration-api-openapi.yml
  format: yaml
  label: Apple Pay Merchant Registration API
  slug: apple-pay-merchant-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apple-pay/refs/heads/main/openapi/apple-pay-merchant-registration-api-openapi.yml
- filename: apple-pay-merchant-validation-api-openapi.yml
  format: yaml
  label: Apple Pay Merchant Validation API
  slug: apple-pay-merchant-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apple-pay/refs/heads/main/openapi/apple-pay-merchant-validation-api-openapi.yml
- filename: apple-pay-payment-processing-api-openapi.yml
  format: yaml
  label: Apple Pay Payment Processing API
  slug: apple-pay-payment-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apple-pay/refs/heads/main/openapi/apple-pay-payment-processing-api-openapi.yml
- filename: apple-pay-payment-status-api-openapi.yml
  format: yaml
  label: Apple Pay Payment Status API
  slug: apple-pay-payment-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apple-pay/refs/heads/main/openapi/apple-pay-payment-status-api-openapi.yml
auth_types:
- mutualTLS
description: ''
kind: authentication
layout: security
method: derived
name: Apple Pay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apple Pay secures its APIs with mutualTLS across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apple Pay
provider_slug: apple-pay
scheme_count: 1
schemes:
- description: Mutual TLS authentication using the Apple Pay Merchant Identity Certificate. The certificate is obtained from the Apple Developer portal and must be associated with the merchant identifier.
  name: merchantCertificate
  sources:
  - openapi/apple-pay-js-openapi.yml
  type: mutualTLS
slug: apple-pay-authentication
source_filename: apple-pay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apple-pay-js-openapi.yml\nsummary:\n  types:\n  - mutualTLS\nschemes:\n- name: merchantCertificate\n  type: mutualTLS\n  description: Mutual TLS authentication using the Apple Pay Merchant Identity Certificate.\n    The certificate is obtained from the Apple Developer portal and must be associated with\n    the merchant identifier.\n  sources:\n  - openapi/apple-pay-js-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apple-pay/refs/heads/main/authentication/apple-pay-authentication.yml
summary_line: mutualTLS · 1 scheme
tags:
- Apple
- Contactless Payments
- Digital Wallet
- E-Commerce
- Mobile Payments
- Payments
---
