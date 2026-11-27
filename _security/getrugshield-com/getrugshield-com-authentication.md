---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getrugshield-com-advisors-api-openapi.yml
  format: yaml
  label: RugShield Advisors API
  slug: getrugshield-com-advisors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getrugshield-com/openapi/getrugshield-com-advisors-api-openapi.yml
- filename: getrugshield-com-docs-api-openapi.yml
  format: yaml
  label: RugShield Docs API
  slug: getrugshield-com-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getrugshield-com/openapi/getrugshield-com-docs-api-openapi.yml
- filename: getrugshield-com-health-api-openapi.yml
  format: yaml
  label: RugShield Health API
  slug: getrugshield-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getrugshield-com/openapi/getrugshield-com-health-api-openapi.yml
- filename: getrugshield-com-jobs-api-openapi.yml
  format: yaml
  label: RugShield Jobs API
  slug: getrugshield-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getrugshield-com/openapi/getrugshield-com-jobs-api-openapi.yml
- filename: getrugshield-com-llms-txt-api-openapi.yml
  format: yaml
  label: RugShield Llms.txt API
  slug: getrugshield-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getrugshield-com/openapi/getrugshield-com-llms-txt-api-openapi.yml
- filename: getrugshield-com-risk-panel-api-openapi.yml
  format: yaml
  label: RugShield Risk Panel API
  slug: getrugshield-com-risk-panel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getrugshield-com/openapi/getrugshield-com-risk-panel-api-openapi.yml
- filename: getrugshield-com-token-risk-api-openapi.yml
  format: yaml
  label: RugShield Token Risk API
  slug: getrugshield-com-token-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getrugshield-com/openapi/getrugshield-com-token-risk-api-openapi.yml
- filename: getrugshield-com-trial-api-openapi.yml
  format: yaml
  label: RugShield Trial API
  slug: getrugshield-com-trial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getrugshield-com/openapi/getrugshield-com-trial-api-openapi.yml
- filename: getrugshield-com-tx-guard-api-openapi.yml
  format: yaml
  label: RugShield Tx Guard API
  slug: getrugshield-com-tx-guard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getrugshield-com/openapi/getrugshield-com-tx-guard-api-openapi.yml
auth_types: []
description: Authentication for RugShield is performed via a custom payment signature header as part of the x402 payment flow.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: RugShield Authentication
name_suffix: Authentication
oauth_flows: []
overview: RugShield declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: RugShield
provider_slug: getrugshield-com
scheme_count: 1
schemes:
- evidence: '"PAYMENT-SIGNATURE": encode_payment_signature_header(payload)'
  header: PAYMENT-SIGNATURE
  how_to_obtain: Obtain a payment quote (HTTP 402 response with a PAYMENT-REQUIRED header), create a payment payload with the wallet, and include the resulting signature in the PAYMENT-SIGNATURE header.
  location: header
  name: x402 payment
  type: other
slug: getrugshield-com-authentication
source_filename: getrugshield-com-authentication.yml
source_heading: Authentication Profile
source_url: https://getrugshield.com/v1/trial/token-risk/So11111111111111111111111111111111111111112
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getrugshield.com/v1/trial/token-risk/So11111111111111111111111111111111111111112\nsources:\n- https://getrugshield.com/v1/trial/token-risk/So11111111111111111111111111111111111111112\n- https://getrugshield.com/docs/payment-client-guide\ndescription: Authentication for RugShield is performed via a custom payment signature header as part of the x402 payment flow.\nschemes:\n- type: other\n  name: x402 payment\n  evidence: '\"PAYMENT-SIGNATURE\": encode_payment_signature_header(payload)'\n  location: header\n  header: PAYMENT-SIGNATURE\n  how_to_obtain: Obtain a payment quote (HTTP 402 response with a PAYMENT-REQUIRED header), create a payment payload with the wallet, and include\n    the resulting signature in the PAYMENT-SIGNATURE header.\ndocs: https://getrugshield.com/v1/trial/token-risk/So11111111111111111111111111111111111111112\n"
source_yaml_url: https://artifacts.apis.io/getrugshield-com/authentication/getrugshield-com-authentication.yml
summary_line: 1 scheme
tags:
- Fintech
- Blockchain
- Solana
- Risk Assessment
---
