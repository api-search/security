---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openpayments-io-account-information-service-ais-api-openapi.yml
  format: yaml
  label: Open Payments Account Information Service (AIS) API
  slug: openpayments-io-account-information-service-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-account-information-service-ais-api-openapi.yml
- filename: openpayments-io-aspsp-information-service-api-openapi.yml
  format: yaml
  label: Open Payments ASPSP Information Service API
  slug: openpayments-io-aspsp-information-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-aspsp-information-service-api-openapi.yml
- filename: openpayments-io-bankgiro-lookup-api-openapi.yml
  format: yaml
  label: Open Payments Bankgiro Lookup API
  slug: openpayments-io-bankgiro-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-bankgiro-lookup-api-openapi.yml
- filename: openpayments-io-consent-service-api-openapi.yml
  format: yaml
  label: Open Payments Consent Service API
  slug: openpayments-io-consent-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-consent-service-api-openapi.yml
- filename: openpayments-io-fx-connect-api-openapi.yml
  format: yaml
  label: Open Payments FX Connect API
  slug: openpayments-io-fx-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-fx-connect-api-openapi.yml
- filename: openpayments-io-iso-payments-api-openapi.yml
  format: yaml
  label: Open Payments ISO Payments API
  slug: openpayments-io-iso-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-iso-payments-api-openapi.yml
- filename: openpayments-io-kyc-service-api-openapi.yml
  format: yaml
  label: Open Payments KYC Service API
  slug: openpayments-io-kyc-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-kyc-service-api-openapi.yml
- filename: openpayments-io-payment-initiation-service-pis-api-openapi.yml
  format: yaml
  label: Open Payments Payment Initiation Service (PIS) API
  slug: openpayments-io-payment-initiation-service-pis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-payment-initiation-service-pis-api-openapi.yml
- filename: openpayments-io-payout-service-api-openapi.yml
  format: yaml
  label: Open Payments Payout Service API
  slug: openpayments-io-payout-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-payout-service-api-openapi.yml
- filename: openpayments-io-sepa-direct-debit-api-openapi.yml
  format: yaml
  label: Open Payments SEPA Direct Debit API
  slug: openpayments-io-sepa-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-sepa-direct-debit-api-openapi.yml
- filename: openpayments-io-verification-of-payee-vop-api-openapi.yml
  format: yaml
  label: Open Payments Verification of Payee (VoP) API
  slug: openpayments-io-verification-of-payee-vop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-verification-of-payee-vop-api-openapi.yml
auth_types: []
description: Authentication for Open Payments API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Openpayments Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open Payments declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Open Payments
provider_slug: openpayments-io
scheme_count: 1
schemes:
- evidence: We use OAuth2 with client credentials for authentication which is a well-known standard.
  flows:
  - client_credentials
  how_to_obtain: Obtain `client_id` and `client_secret` by creating an application in the Developer Portal (sandbox or production). Use them in a POST request to the token endpoint with `grant_type=client_credentials` and the desired `scope`.
  name: OAuth2
  scopes:
  - aspspinformation
  - accountinformation
  - paymentinitiation
  - bankgiroinformation
  - private
  - corporate
  token_url: https://auth.openbankingplatform.com/connect/token
  type: oauth2
slug: openpayments-io-authentication
source_filename: openpayments-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.openpayments.io/docs/get_access_token.md
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.openpayments.io/docs/get_access_token.md\nsources:\n- https://docs.openpayments.io/docs/get_access_token.md\n- https://docs.openpayments.io/docs/getstarted.md\n- https://docs.openpayments.io/docs/quickstart_pis.md\ndescription: Authentication for Open Payments API\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: We use OAuth2 with client credentials for authentication which is a well-known standard.\n  flows:\n  - client_credentials\n  token_url: https://auth.openbankingplatform.com/connect/token\n  scopes:\n  - aspspinformation\n  - accountinformation\n  - paymentinitiation\n  - bankgiroinformation\n  - private\n  - corporate\n  how_to_obtain: Obtain `client_id` and `client_secret` by creating an application in the Developer Portal (sandbox or production). Use them in\n    a POST request to the token endpoint with `grant_type=client_credentials` and the desired\
  \ `scope`.\nnote: All API requests must include the access token in the `Authorization` header as `Bearer <ACCESS_TOKEN>`.\ndocs: https://docs.openpayments.io/docs/get_access_token.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/authentication/openpayments-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payments
- Banking
- Fintech
---
