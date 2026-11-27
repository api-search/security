---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: code402-dev-autonomous-api-openapi.yml
  format: yaml
  label: Code402 Autonomous API
  slug: code402-dev-autonomous-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-autonomous-api-openapi.yml
- filename: code402-dev-fx-api-openapi.yml
  format: yaml
  label: Code402 Fx API
  slug: code402-dev-fx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-fx-api-openapi.yml
- filename: code402-dev-modules-api-openapi.yml
  format: yaml
  label: Code402 Modules API
  slug: code402-dev-modules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-modules-api-openapi.yml
- filename: code402-dev-multimodal-api-openapi.yml
  format: yaml
  label: Code402 Multimodal API
  slug: code402-dev-multimodal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-multimodal-api-openapi.yml
- filename: code402-dev-quota-api-openapi.yml
  format: yaml
  label: Code402 Quota API
  slug: code402-dev-quota-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-quota-api-openapi.yml
- filename: code402-dev-receipt-api-openapi.yml
  format: yaml
  label: Code402 Receipt API
  slug: code402-dev-receipt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-receipt-api-openapi.yml
- filename: code402-dev-tools-api-openapi.yml
  format: yaml
  label: Code402 Tools API
  slug: code402-dev-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-tools-api-openapi.yml
- filename: code402-dev-webhooks-api-openapi.yml
  format: yaml
  label: Code402 Webhooks API
  slug: code402-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/code402-dev/openapi/code402-dev-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Code402 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Code402 secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Code402
provider_slug: code402-dev
scheme_count: 4
schemes:
- description: Prepaid non-custodial quota key (ck_live_...) purchased at https://hcrb.in/checkout
  docs_quote: 'Existing credit keys still use Authorization: Bearer ck_… .'
  name: OperatorQuotaBearer
  scheme: bearer
  sources:
  - openapi/code402-dev-openapi.yml
  - https://code402.dev/docs
  type: http
- description: Base64-encoded EIP-3009 transferWithAuthorization voucher on Base (eip155:8453)
  docs_quote: 'x402 v2 HTTP: decode PAYMENT-REQUIRED; an authorized client sends PAYMENT-SIGNATURE; inspect PAYMENT-RESPONSE. Legacy X-PAYMENT compatibility is separate from the v2 format.'
  in: header
  name: X402PaymentSignature
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/code402-dev-openapi.yml
  - https://hcrb.in/llms.txt
  type: apiKey
- description: 'Docs: "mint a trial key (5-minute bearer, larger budget) and send it as Authorization: Bearer <trial-key>", minted via POST https://hcrb.in/api/auth/ephemeral-key. Not declared in the OpenAPI; not called by this pipeline.'
  documented_only: true
  name: TrialKey
  scheme: bearer
  sources:
  - https://code402.dev/docs
  type: http
- description: 'llms.txt: GET https://hcrb.in/entitlement with header "Authorization: Bearer ek_..."'
  documented_only: true
  name: EntitlementKey
  scheme: bearer
  sources:
  - https://hcrb.in/llms.txt
  type: http
slug: code402-dev-authentication
source_filename: code402-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- openapi/code402-dev-openapi.yml\n- https://code402.dev/docs\n- https://hcrb.in/llms.txt\ndocs: https://code402.dev/docs\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: OperatorQuotaBearer\n  type: http\n  scheme: bearer\n  description: Prepaid non-custodial quota key (ck_live_...) purchased at https://hcrb.in/checkout\n  docs_quote: 'Existing credit keys still use Authorization: Bearer ck_… .'\n  sources:\n  - openapi/code402-dev-openapi.yml\n  - https://code402.dev/docs\n- name: X402PaymentSignature\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: Base64-encoded EIP-3009 transferWithAuthorization voucher on Base (eip155:8453)\n  docs_quote: 'x402 v2 HTTP: decode PAYMENT-REQUIRED; an authorized client sends PAYMENT-SIGNATURE; inspect PAYMENT-RESPONSE. Legacy X-PAYMENT compatibility is separate from the v2 format.'\n  sources:\n  - openapi/code402-dev-openapi.yml\n\
  \  - https://hcrb.in/llms.txt\n- name: TrialKey\n  type: http\n  scheme: bearer\n  documented_only: true\n  description: 'Docs: \"mint a trial key (5-minute bearer, larger budget) and send it as Authorization: Bearer <trial-key>\", minted via POST https://hcrb.in/api/auth/ephemeral-key. Not declared in the OpenAPI;\n    not called by this pipeline.'\n  sources:\n  - https://code402.dev/docs\n- name: EntitlementKey\n  type: http\n  scheme: bearer\n  documented_only: true\n  description: 'llms.txt: GET https://hcrb.in/entitlement with header \"Authorization: Bearer ek_...\"'\n  sources:\n  - https://hcrb.in/llms.txt\nunauthenticated_access: A daily free allowance is available without a wallet; MCP \"no key needed to start\".\nkey_formats:\n- ck_live_\n- ek_\n"
source_yaml_url: https://artifacts.apis.io/code402-dev/authentication/code402-dev-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Payments
- Reconciliation
- x402
- AI Agents
- Verification
- MCP
- ISO 20022
---
