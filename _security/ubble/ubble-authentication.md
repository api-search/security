---
api_key_in: []
api_specs:
- filename: ubble-address-document-verifications-coming-soon-api-openapi.yml
  format: yaml
  label: Ubble Address document verifications (Coming soon) API
  slug: ubble-address-document-verifications-coming-soon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubble/refs/heads/main/openapi/ubble-address-document-verifications-coming-soon-api-openapi.yml
- filename: ubble-aml-verifications-api-openapi.yml
  format: yaml
  label: Ubble AML verifications API
  slug: ubble-aml-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubble/refs/heads/main/openapi/ubble-aml-verifications-api-openapi.yml
- filename: ubble-applicants-api-openapi.yml
  format: yaml
  label: Ubble Applicants API
  slug: ubble-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubble/refs/heads/main/openapi/ubble-applicants-api-openapi.yml
- filename: ubble-bank-document-verifications-coming-soon-api-openapi.yml
  format: yaml
  label: Ubble Bank document verifications (Coming soon) API
  slug: ubble-bank-document-verifications-coming-soon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubble/refs/heads/main/openapi/ubble-bank-document-verifications-coming-soon-api-openapi.yml
- filename: ubble-business-applicants-api-openapi.yml
  format: yaml
  label: Ubble Business applicants API
  slug: ubble-business-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubble/refs/heads/main/openapi/ubble-business-applicants-api-openapi.yml
- filename: ubble-company-document-verifications-coming-soon-api-openapi.yml
  format: yaml
  label: Ubble Company document verifications (Coming soon) API
  slug: ubble-company-document-verifications-coming-soon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubble/refs/heads/main/openapi/ubble-company-document-verifications-coming-soon-api-openapi.yml
- filename: ubble-face-authentications-api-openapi.yml
  format: yaml
  label: Ubble Face authentications API
  slug: ubble-face-authentications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubble/refs/heads/main/openapi/ubble-face-authentications-api-openapi.yml
- filename: ubble-id-document-verifications-api-openapi.yml
  format: yaml
  label: Ubble ID document verifications API
  slug: ubble-id-document-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubble/refs/heads/main/openapi/ubble-id-document-verifications-api-openapi.yml
- filename: ubble-identity-verifications-api-openapi.yml
  format: yaml
  label: Ubble Identity verifications API
  slug: ubble-identity-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubble/refs/heads/main/openapi/ubble-identity-verifications-api-openapi.yml
- filename: ubble-service-status-api-openapi.yml
  format: yaml
  label: Ubble Service status API
  slug: ubble-service-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubble/refs/heads/main/openapi/ubble-service-status-api-openapi.yml
- filename: ubble-website-verifications-coming-soon-api-openapi.yml
  format: yaml
  label: Ubble Website verifications (Coming soon) API
  slug: ubble-website-verifications-coming-soon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubble/refs/heads/main/openapi/ubble-website-verifications-coming-soon-api-openapi.yml
auth_types:
- http-basic
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Ubble Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ubble secures its APIs with http-basic and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ubble
provider_slug: ubble
scheme_count: 2
schemes:
- description: HTTP Basic authentication using API credentials managed in the client dashboard or by the account manager (legacy v1 reference; standard accounts).
  name: basicAuth
  scheme: basic
  sources:
  - https://ubbleai.github.io/developer-documentation/#basic-authentication
  type: http
- description: Mutual TLS authentication. The v2 documentation instructs clients to include their mTLS certificate in all API calls; in the legacy v1 reference mTLS is required for certified accounts in addition to Basic authentication.
  name: mutualTLS
  sources:
  - https://docs.ubble.ai/docs/introduction/before-you-begin
  - https://ubbleai.github.io/developer-documentation/#mutual-tls-authentication
  type: mutualTLS
slug: ubble-authentication
source_filename: ubble-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.ubble.ai/docs/introduction/before-you-begin\ndocs:\n  - https://docs.ubble.ai/docs/introduction/before-you-begin\n  - https://ubbleai.github.io/developer-documentation/#authentication\n  - https://docs.ubble.ai/docs/api-standard/signature\nsummary:\n  types: [http-basic, mutualTLS]\n  api_key_in: []\n  oauth2_flows: []\nnotes: >-\n  The published OpenAPI 3.0.3 contract declares no components.securitySchemes; the\n  authentication model is documented in the developer docs. API credentials are\n  created in the client dashboard (https://dashboard.ubble.ai/). The v2 docs\n  instruct clients to include an mTLS certificate in all API calls; the legacy v1\n  reference documents HTTP Basic authentication for standard accounts, with mutual\n  TLS added on top for certified accounts. Webhook notifications and (optionally)\n  API responses are signed with ECDSA/SHA-512 via the Cko-Signature header.\nschemes:\n  - name: basicAuth\n\
  \    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication using API credentials managed in the client\n      dashboard or by the account manager (legacy v1 reference; standard accounts).\n    sources:\n      - https://ubbleai.github.io/developer-documentation/#basic-authentication\n  - name: mutualTLS\n    type: mutualTLS\n    description: >-\n      Mutual TLS authentication. The v2 documentation instructs clients to include\n      their mTLS certificate in all API calls; in the legacy v1 reference mTLS is\n      required for certified accounts in addition to Basic authentication.\n    sources:\n      - https://docs.ubble.ai/docs/introduction/before-you-begin\n      - https://ubbleai.github.io/developer-documentation/#mutual-tls-authentication\nresponse_signing:\n  header: Cko-Signature\n  algorithm: ECDSA with SHA-512\n  format: '<timestamp>:<organization_id>-<test or live verification>-<key version>:<signature>'\n  public_keys: https://dashboard.ubble.ai/security\
  \ (separate keys for test and live environments)\n  scope: Webhook notifications are signed by default; API response signing is enabled on request.\n  code_samples: https://github.com/ubbleai/code-samples\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubble/refs/heads/main/authentication/ubble-authentication.yml
summary_line: http-basic/mutualTLS · 2 schemes
tags:
- Company
- Identity Verification
- KYC
- AML
- Biometrics
- Face Authentication
- Document Verification
- Fraud Prevention
- Compliance
- Fintech
---
