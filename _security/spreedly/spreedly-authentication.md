---
api_key_in: []
api_specs:
- filename: spreedly-api-v1.json
  format: json
  label: Spreedly Core Transactional API
  slug: spreedly-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/openapi/spreedly-api-v1.json
- filename: spreedly-api-v1.json
  format: json
  label: Spreedly Payment Methods & Vault API
  slug: spreedly-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/openapi/spreedly-api-v1.json
- filename: spreedly-api-v1.json
  format: json
  label: Spreedly Composer (Workflows) API
  slug: spreedly-composer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/openapi/spreedly-api-v1.json
- filename: spreedly-api-v1.json
  format: json
  label: Spreedly Network Tokenization API
  slug: spreedly-network-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/openapi/spreedly-api-v1.json
- filename: spreedly-api-v1.json
  format: json
  label: Spreedly Account Updater (Card Refresher) API
  slug: spreedly-account-updater-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/openapi/spreedly-api-v1.json
- filename: spreedly-api-v1.json
  format: json
  label: Spreedly Receivers API
  slug: spreedly-receivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/openapi/spreedly-api-v1.json
- filename: spreedly-api-v1.json
  format: json
  label: Spreedly 3-D Secure / SCA Authentication API
  slug: spreedly-sca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/openapi/spreedly-api-v1.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Spreedly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spreedly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spreedly
provider_slug: spreedly
scheme_count: 1
schemes:
- description: "Unless otherwise noted, all calls to the Spreedly API use [HTTP basic authentication](https://en.wikipedia.org/wiki/Basic_access_authentication) over HTTPS.\n            Use the [environment key](https://developer.spreedly.com/docs/the-spreedly-app#environment-key) of the Spreedly environment you wish to execute against as the HTTP basic user, and one of your organization's [access secrets](https:/"
  name: basic_auth
  scheme: basic
  sources:
  - openapi/spreedly-api-v1.json
  type: http
slug: spreedly-authentication
source_filename: spreedly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/spreedly-api-v1.json\ndocs: https://developer.spreedly.com/docs/the-spreedly-app#environment-key\nsummary:\n  types:\n  - http\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  description: |-\n    Unless otherwise noted, all calls to the Spreedly API use [HTTP basic authentication](https://en.wikipedia.org/wiki/Basic_access_authentication) over HTTPS.\n                Use the [environment key](https://developer.spreedly.com/docs/the-spreedly-app#environment-key) of the Spreedly environment you wish to execute against as the HTTP basic user, and one of your organization's [access secrets](https:/\n  sources:\n  - openapi/spreedly-api-v1.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spreedly/refs/heads/main/authentication/spreedly-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- United States
- Payment Gateway
- Payment Orchestration
- Payment Processing
- Card Vault
- Tokenization
- Network Tokenization
- PCI Compliance
- Subscription
---
