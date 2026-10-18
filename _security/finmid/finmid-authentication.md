---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: finmid-beta-endpoints-api-openapi.yml
  format: yaml
  label: Finmid Beta Endpoints API
  slug: finmid-beta-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-beta-endpoints-api-openapi.yml
- filename: finmid-business-api-openapi.yml
  format: yaml
  label: Finmid Business API
  slug: finmid-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-business-api-openapi.yml
- filename: finmid-buyer-api-openapi.yml
  format: yaml
  label: Finmid Buyer API
  slug: finmid-buyer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-buyer-api-openapi.yml
- filename: finmid-capital-max-api-openapi.yml
  format: yaml
  label: Finmid Capital Max API
  slug: finmid-capital-max-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-capital-max-api-openapi.yml
- filename: finmid-csp-financial-document-api-openapi.yml
  format: yaml
  label: Finmid CSP Financial Document API
  slug: finmid-csp-financial-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-csp-financial-document-api-openapi.yml
- filename: finmid-document-api-openapi.yml
  format: yaml
  label: Finmid Document API
  slug: finmid-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-document-api-openapi.yml
- filename: finmid-funding-api-openapi.yml
  format: yaml
  label: Finmid Funding API
  slug: finmid-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-funding-api-openapi.yml
- filename: finmid-funding-application-api-openapi.yml
  format: yaml
  label: Finmid Funding Application API
  slug: finmid-funding-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-funding-application-api-openapi.yml
- filename: finmid-incoming-webhook-api-openapi.yml
  format: yaml
  label: Finmid Incoming Webhook API
  slug: finmid-incoming-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-incoming-webhook-api-openapi.yml
- filename: finmid-offer-api-openapi.yml
  format: yaml
  label: Finmid Offer API
  slug: finmid-offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-offer-api-openapi.yml
- filename: finmid-offer-group-api-openapi.yml
  format: yaml
  label: Finmid Offer Group API
  slug: finmid-offer-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-offer-group-api-openapi.yml
- filename: finmid-onboarding-api-openapi.yml
  format: yaml
  label: Finmid Onboarding API
  slug: finmid-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-onboarding-api-openapi.yml
- filename: finmid-payment-api-openapi.yml
  format: yaml
  label: Finmid Payment API
  slug: finmid-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-payment-api-openapi.yml
- filename: finmid-payment-request-api-openapi.yml
  format: yaml
  label: Finmid Payment Request API
  slug: finmid-payment-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-payment-request-api-openapi.yml
- filename: finmid-sales-statements-api-openapi.yml
  format: yaml
  label: Finmid Sales statements API
  slug: finmid-sales-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-sales-statements-api-openapi.yml
- filename: finmid-seller-api-openapi.yml
  format: yaml
  label: Finmid Seller API
  slug: finmid-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-seller-api-openapi.yml
- filename: finmid-simulation-api-openapi.yml
  format: yaml
  label: Finmid Simulation API
  slug: finmid-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-simulation-api-openapi.yml
- filename: finmid-tasks-api-openapi.yml
  format: yaml
  label: Finmid Tasks API
  slug: finmid-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/openapi/finmid-tasks-api-openapi.yml
auth_types:
- apiKey
- httpMessageSignatures
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Finmid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Finmid secures its APIs with apiKey and httpMessageSignatures across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Finmid
provider_slug: finmid
scheme_count: 2
schemes:
- applies_to:
  - B2B Payments API
  - Capital API
  description: Primary authentication for both the B2B Payments API and the Capital API. Every request must include the X-API-Key header. Keys are environment specific — a sandbox key (https://sandbox.finmid.com) cannot access live data and a live key (https://api.finmid.com) cannot access sandbox data. Keys are managed in the finmid Dashboard.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  type: apiKey
- algorithm: Ed25519
  applies_to:
  - Capital API - platform-provided capital
  description: For platform-provided capital, the Execute Payment Transaction endpoint (platform-initiated payouts) is additionally protected with HTTP Message Signatures (RFC 9421). Requests are signed with Ed25519, include a Content-Digest for body integrity, use temporal/replay-attack prevention, and require IP whitelisting.
  name: HttpMessageSignatures
  standard: RFC 9421
  type: http-message-signatures
slug: finmid-authentication
source_filename: finmid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.finmid.com/reference/api-introduction\ndocs: https://docs.finmid.com/reference/api-introduction\nsummary:\n  types: [apiKey, httpMessageSignatures]\n  api_key_in: [header]\n  api_key_name: X-API-Key\n  environments: [sandbox, live]\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: >-\n    Primary authentication for both the B2B Payments API and the Capital API.\n    Every request must include the X-API-Key header. Keys are environment\n    specific — a sandbox key (https://sandbox.finmid.com) cannot access live\n    data and a live key (https://api.finmid.com) cannot access sandbox data.\n    Keys are managed in the finmid Dashboard.\n  applies_to: [B2B Payments API, Capital API]\n- name: HttpMessageSignatures\n  type: http-message-signatures\n  standard: RFC 9421\n  algorithm: Ed25519\n  description: >-\n    For platform-provided capital, the Execute Payment Transaction\
  \ endpoint\n    (platform-initiated payouts) is additionally protected with HTTP Message\n    Signatures (RFC 9421). Requests are signed with Ed25519, include a\n    Content-Digest for body integrity, use temporal/replay-attack prevention,\n    and require IP whitelisting.\n  applies_to: [Capital API - platform-provided capital]\nwebhook_auth:\n  description: >-\n    Inbound webhooks from finmid to your endpoint use HTTP Basic authentication\n    plus an HMAC-SHA-256 payload signature carried in the X-Payload-Signature\n    header (Base64-encoded), verified with a per-endpoint signature_secret.\n  source: https://docs.finmid.com/docs/webhooks\nnotes:\n- OAuth 2.0 / OpenID Connect are not used — authentication is API-key based.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finmid/refs/heads/main/authentication/finmid-authentication.yml
summary_line: apiKey/httpMessageSignatures · 2 schemes
tags:
- Company
- Embedded Finance
- Embedded Lending
- B2B Payments
- Fintech
- Lending
- Capital
- Financing
- Payments
- Marketplace
---
