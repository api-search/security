---
api_key_in: []
api_specs:
- filename: finix-authorizations-api-openapi.yml
  format: yaml
  label: Finix Authorizations API
  slug: finix-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-authorizations-api-openapi.yml
- filename: finix-balance-transfers-api-openapi.yml
  format: yaml
  label: Finix Balance Transfers API
  slug: finix-balance-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-balance-transfers-api-openapi.yml
- filename: finix-compliance-forms-api-openapi.yml
  format: yaml
  label: Finix Compliance Forms API
  slug: finix-compliance-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-compliance-forms-api-openapi.yml
- filename: finix-devices-api-openapi.yml
  format: yaml
  label: Finix Devices API
  slug: finix-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-devices-api-openapi.yml
- filename: finix-disputes-api-openapi.yml
  format: yaml
  label: Finix Disputes API
  slug: finix-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-disputes-api-openapi.yml
- filename: finix-fee-profiles-api-openapi.yml
  format: yaml
  label: Finix Fee Profiles API
  slug: finix-fee-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-fee-profiles-api-openapi.yml
- filename: finix-files-api-openapi.yml
  format: yaml
  label: Finix Files API
  slug: finix-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-files-api-openapi.yml
- filename: finix-identities-api-openapi.yml
  format: yaml
  label: Finix Identities API
  slug: finix-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-identities-api-openapi.yml
- filename: finix-instrument-updates-api-openapi.yml
  format: yaml
  label: Finix Instrument Updates API
  slug: finix-instrument-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-instrument-updates-api-openapi.yml
- filename: finix-merchant-profiles-api-openapi.yml
  format: yaml
  label: Finix Merchant Profiles API
  slug: finix-merchant-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-merchant-profiles-api-openapi.yml
- filename: finix-merchants-api-openapi.yml
  format: yaml
  label: Finix Merchants API
  slug: finix-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-merchants-api-openapi.yml
- filename: finix-onboarding-forms-api-openapi.yml
  format: yaml
  label: Finix Onboarding Forms API
  slug: finix-onboarding-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-onboarding-forms-api-openapi.yml
- filename: finix-payment-instruments-api-openapi.yml
  format: yaml
  label: Finix Payment Instruments API
  slug: finix-payment-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-payment-instruments-api-openapi.yml
- filename: finix-payout-profiles-api-openapi.yml
  format: yaml
  label: Finix Payout Profiles API
  slug: finix-payout-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-payout-profiles-api-openapi.yml
- filename: finix-settlements-api-openapi.yml
  format: yaml
  label: Finix Settlements API
  slug: finix-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-settlements-api-openapi.yml
- filename: finix-split-transfers-api-openapi.yml
  format: yaml
  label: Finix Split Transfers API
  slug: finix-split-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-split-transfers-api-openapi.yml
- filename: finix-transfers-api-openapi.yml
  format: yaml
  label: Finix Transfers API
  slug: finix-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-transfers-api-openapi.yml
- filename: finix-verifications-api-openapi.yml
  format: yaml
  label: Finix Verifications API
  slug: finix-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-verifications-api-openapi.yml
- filename: finix-webhooks-api-openapi.yml
  format: yaml
  label: Finix Webhooks API
  slug: finix-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/openapi/finix-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Finix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Finix
provider_slug: finix
scheme_count: 1
schemes:
- header: 'Authorization: Basic <Base64(username:password)>'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/finix-openapi-original.yml
  type: http
slug: finix-authentication
source_filename: finix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/finix-openapi-original.yml\ndocs: https://docs.finix.com/additional-resources/developers/authentication-and-api-basics/api-keys\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  standard: RFC 7617 HTTP Basic Authentication\n  key_model: API key ID (username) + API key secret (password), Base64-encoded in the Authorization header\n  environment_separation: Sandbox keys and Live keys are not interchangeable; each is issued from its own dashboard\nroles:\n- name: ROLE_PLATFORM\n  description: Highest access. Access all Applications and Merchant data, create Applications and Merchants, and assign roles.\n- name: ROLE_PARTNER\n  description: Access to one Application and its Merchant data.\n- name: ROLE_MERCHANT\n  description: Access to a single Merchant and its data.\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  header: 'Authorization: Basic <Base64(username:password)>'\n  sources:\n  - openapi/finix-openapi-original.yml\n\
  notes:\n- Combine the API key username and password with a colon and Base64-encode, per RFC 7617.\n- The optional finix-apiuser-role header can scope a request to a specific role.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finix/refs/heads/main/authentication/finix-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fintech
- Payments
- Payment Processing
- Payment Facilitation
- Merchant Onboarding
- Payouts
- Marketplaces
---
