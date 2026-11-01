---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gnosis-pay-auth-api-openapi.yml
  format: yaml
  label: Gnosis Pay Auth API
  slug: gnosis-pay-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-auth-api-openapi.yml
- filename: gnosis-pay-cards-api-openapi.yml
  format: yaml
  label: Gnosis Pay Cards API
  slug: gnosis-pay-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-cards-api-openapi.yml
- filename: gnosis-pay-health-api-openapi.yml
  format: yaml
  label: Gnosis Pay Health API
  slug: gnosis-pay-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-health-api-openapi.yml
- filename: gnosis-pay-kyc-api-openapi.yml
  format: yaml
  label: Gnosis Pay KYC API
  slug: gnosis-pay-kyc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-kyc-api-openapi.yml
- filename: gnosis-pay-pci-api-openapi.yml
  format: yaml
  label: Gnosis Pay PCI API
  slug: gnosis-pay-pci-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-pci-api-openapi.yml
- filename: gnosis-pay-phone-api-openapi.yml
  format: yaml
  label: Gnosis Pay Phone API
  slug: gnosis-pay-phone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-phone-api-openapi.yml
- filename: gnosis-pay-source-of-funds-api-openapi.yml
  format: yaml
  label: Gnosis Pay Source of Funds API
  slug: gnosis-pay-source-of-funds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-source-of-funds-api-openapi.yml
- filename: gnosis-pay-terms-api-openapi.yml
  format: yaml
  label: Gnosis Pay Terms API
  slug: gnosis-pay-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-terms-api-openapi.yml
- filename: gnosis-pay-user-account-api-openapi.yml
  format: yaml
  label: Gnosis Pay User Account API
  slug: gnosis-pay-user-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-user-account-api-openapi.yml
- filename: gnosis-pay-user-api-openapi.yml
  format: yaml
  label: Gnosis Pay User API
  slug: gnosis-pay-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-user-api-openapi.yml
- filename: gnosis-pay-user-movements-api-openapi.yml
  format: yaml
  label: Gnosis Pay User Movements API
  slug: gnosis-pay-user-movements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-user-movements-api-openapi.yml
- filename: gnosis-pay-3-ds-api-openapi.yml
  format: yaml
  label: Gnosis Pay 3 DS API
  slug: gnosis-pay-3-ds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosis-pay/openapi/gnosis-pay-3-ds-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Gnosis Pay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gnosis Pay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gnosis Pay
provider_slug: gnosis-pay
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: Bearer
  sources:
  - openapi/gnosis-pay-openapi.json
  type: http
slug: gnosis-pay-authentication
source_filename: gnosis-pay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: derived\nsource: openapi/gnosis-pay-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: Bearer\n  sources:\n  - openapi/gnosis-pay-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/gnosis-pay/authentication/gnosis-pay-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- Crypto
- Stablecoin
- API
---
