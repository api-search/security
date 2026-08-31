---
api_key_in:
- header
api_specs:
- filename: faturapdf-brazilian-invoice-receipt-pdf-api-documents-api-openapi.yml
  format: yaml
  label: FaturaPDF — Brazilian Invoice & Receipt PDF API Documents API
  slug: faturapdf-brazilian-invoice-receipt-pdf-api-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faturapdf-brazilian-invoice-receipt-pdf-api/refs/heads/main/openapi/faturapdf-brazilian-invoice-receipt-pdf-api-documents-api-openapi.yml
auth_types:
- apiKey
description: A single API key in a header, issued and validated by the RapidAPI gateway. FaturaPDF issues no credentials of its own, stores no accounts, and cannot rotate or revoke a key — that is entirely RapidAPI's surface. Derived from the OpenAPI securitySchemes and upgraded from the provider's api-onboarding descriptor (aod 0.1) and integration guides.
kind: authentication
layout: security
method: searched
name: Faturapdf Brazilian Invoice Receipt Pdf Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: FaturaPDF — Brazilian Invoice & Receipt PDF API secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FaturaPDF — Brazilian Invoice & Receipt PDF API
provider_slug: faturapdf-brazilian-invoice-receipt-pdf-api
scheme_count: 2
schemes:
- description: The consumer's personal RapidAPI application key — the only credential a consumer of this API sends. Obtained by subscribing to any plan (including the free 20 documents/month Basic plan, which asks for no card) on the RapidAPI listing; the key is shown immediately in the request builder. A missing or invalid key is rejected by the gateway with HTTP 401.
  env: RAPIDAPI_KEY
  in: header
  name: RapidAPIKey
  parameter: X-RapidAPI-Key
  required: true
  sources:
  - openapi/faturapdf-brazilian-invoice-receipt-pdf-api-openapi-original.yml
  type: apiKey
- description: Optional companion header, always present in RapidAPI's generated code snippets. Accepted and recommended for compatibility with RapidAPI SDKs, but not required when addressing the gateway subdomain directly — X-RapidAPI-Key alone is sufficient, which the provider states was verified against the live gateway.
  in: header
  name: RapidAPIHost
  parameter: X-RapidAPI-Host
  required: false
  sources:
  - openapi/faturapdf-brazilian-invoice-receipt-pdf-api-openapi-original.yml
  type: apiKey
  value: brazilian-invoice-receipt-pdf-api-cpf-cnpj.p.rapidapi.com
slug: faturapdf-brazilian-invoice-receipt-pdf-api-authentication
source_filename: faturapdf-brazilian-invoice-receipt-pdf-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/faturapdf-brazilian-invoice-receipt-pdf-api-openapi-original.yml\ndocs:\n  - https://faturapdf.com/.well-known/api-onboarding\n  - https://faturapdf.com/guides/generate-invoice-pdf-nodejs/\n  - https://faturapdf.com/terms/\ndescription: >-\n  A single API key in a header, issued and validated by the RapidAPI gateway. FaturaPDF issues\n  no credentials of its own, stores no accounts, and cannot rotate or revoke a key — that is\n  entirely RapidAPI's surface. Derived from the OpenAPI securitySchemes and upgraded from the\n  provider's api-onboarding descriptor (aod 0.1) and integration guides.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows: []\nschemes:\n  - name: RapidAPIKey\n    type: apiKey\n    in: header\n    parameter: X-RapidAPI-Key\n    required: true\n    env: RAPIDAPI_KEY\n    description: >-\n      The consumer's personal RapidAPI application key — the only credential a consumer\
  \ of this\n      API sends. Obtained by subscribing to any plan (including the free 20 documents/month\n      Basic plan, which asks for no card) on the RapidAPI listing; the key is shown immediately\n      in the request builder. A missing or invalid key is rejected by the gateway with HTTP 401.\n    sources:\n      - openapi/faturapdf-brazilian-invoice-receipt-pdf-api-openapi-original.yml\n  - name: RapidAPIHost\n    type: apiKey\n    in: header\n    parameter: X-RapidAPI-Host\n    required: false\n    value: brazilian-invoice-receipt-pdf-api-cpf-cnpj.p.rapidapi.com\n    description: >-\n      Optional companion header, always present in RapidAPI's generated code snippets. Accepted\n      and recommended for compatibility with RapidAPI SDKs, but not required when addressing the\n      gateway subdomain directly — X-RapidAPI-Key alone is sufficient, which the provider states\n      was verified against the live gateway.\n    sources:\n      - openapi/faturapdf-brazilian-invoice-receipt-pdf-api-openapi-original.yml\n\
  applied_to: >-\n  Global security requirement — every operation, including healthCheck, requires RapidAPIKey when\n  called through the gateway.\nissuance:\n  owner: RapidAPI\n  application_noun: API key\n  mechanism: marketplace subscription (self-serve)\n  signup: https://rapidapi.com/leosanchees2014/api/brazilian-invoice-receipt-pdf-api-cpf-cnpj\n  one_time_display: false\n  rotation: >-\n    Rotate or revoke from the RapidAPI dashboard. FaturaPDF neither issues nor stores keys and\n    cannot help with rotation, quota or refunds.\nscopes:\n  model: quota-tiers\n  note: >-\n    No per-scope permissions exist. Every plan, including the free one, reaches both endpoints and\n    every field; tiers gate monthly document volume only. No scopes/ artifact is emitted.\norigin_enforcement:\n  detail: >-\n    The origin host faturapdf.com is not directly callable. Requests that did not arrive through\n    the RapidAPI gateway are rejected with HTTP 401 {\"error\":\"unauthorized\"}. Internally\
  \ the\n    gateway injects a private proxy secret so the origin can reject non-gateway traffic; that\n    header is never set by, visible to, or relevant for the consumer, and the provider\n    deliberately excludes it from the public contract.\n  public_exception: >-\n    https://faturapdf.com/health is public and unauthenticated on the origin — the one endpoint\n    reachable without a key.\nclient_side_use:\n  allowed: false\n  reason: >-\n    Server-side credential. CORS is not configured for arbitrary origins, and shipping the key to\n    a browser bundle lets anyone spend the quota. Proxy through your own backend. A keyless,\n    fully client-side alternative exists for one-off documents at https://faturapdf.com/gerador.html.\nagent_policy: allowed\nagent_policy_source: >-\n  https://faturapdf.com/.well-known/api-onboarding — account.agentPolicy \"allowed\"; the terms page\n  states \"Automated use is expected and welcome — it is an API — within the quota of your plan.\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/faturapdf-brazilian-invoice-receipt-pdf-api/refs/heads/main/authentication/faturapdf-brazilian-invoice-receipt-pdf-api-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Invoices
- Receipts
- PDF Generation
- Documents
- Brazil
- Billing
- CPF Validation
- CNPJ Validation
- PIX
- Fintech
- Data Validation
---
