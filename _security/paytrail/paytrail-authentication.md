---
anonymous_access: false
api_key_in: []
api_specs:
- filename: paytrail-payment-reports-api-openapi.yml
  format: yaml
  label: Paytrail payment reports API
  slug: paytrail-payment-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paytrail/openapi/paytrail-payment-reports-api-openapi.yml
- filename: paytrail-payments-api-openapi.yml
  format: yaml
  label: Paytrail Payments API
  slug: paytrail-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paytrail/openapi/paytrail-payments-api-openapi.yml
- filename: paytrail-providers-api-openapi.yml
  format: yaml
  label: Paytrail Providers API
  slug: paytrail-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paytrail/openapi/paytrail-providers-api-openapi.yml
- filename: paytrail-settlements-api-openapi.yml
  format: yaml
  label: Paytrail Settlements API
  slug: paytrail-settlements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paytrail/openapi/paytrail-settlements-api-openapi.yml
- filename: paytrail-token-payments-api-openapi.yml
  format: yaml
  label: Paytrail token payments API
  slug: paytrail-token-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paytrail/openapi/paytrail-token-payments-api-openapi.yml
auth_types: []
description: All API calls need to be signed using HMAC and SHA-256 or SHA-512.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Paytrail Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paytrail declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Paytrail
provider_slug: paytrail
scheme_count: 1
schemes:
- evidence: All API calls need to be signed using HMAC and SHA-256 or SHA-512.
  header: signature
  how_to_obtain: 'Merchant ID and Secret key are provided in the Test credentials section (e.g., Merchant ID: 375917, Secret key: SAIPPUAKAUPPIAS).'
  location: header
  name: HMAC
  type: hmac
slug: paytrail-authentication
source_filename: paytrail-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.paytrail.com/#/?id=authentication
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.paytrail.com/#/?id=authentication\nsources:\n- https://docs.paytrail.com/#/?id=authentication\n- https://docs.paytrail.com/#/?id=token-payments\n- https://docs.paytrail.com/#/?id=test-credentials\n- https://docs.paytrail.com/#/?id=redirect-and-callback-url-signing\ndescription: All API calls need to be signed using HMAC and SHA-256 or SHA-512.\nschemes:\n- type: hmac\n  name: HMAC\n  evidence: All API calls need to be signed using HMAC and SHA-256 or SHA-512.\n  location: header\n  header: signature\n  how_to_obtain: 'Merchant ID and Secret key are provided in the Test credentials section (e.g., Merchant ID: 375917, Secret key: SAIPPUAKAUPPIAS).'\nnote: No OAuth2, API key, or other authentication schemes are documented.\ndocs: https://docs.paytrail.com/#/?id=authentication\n"
source_yaml_url: https://artifacts.apis.io/paytrail/authentication/paytrail-authentication.yml
summary_line: 1 scheme
tags:
- Payments
- Fintech
- E-Commerce
- Omnichannel
- Finland
---
