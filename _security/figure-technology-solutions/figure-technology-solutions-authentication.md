---
api_key_in:
- header
api_specs:
- filename: figure-technology-solutions-encryption-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions Encryption API
  slug: figure-technology-solutions-encryption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-encryption-api-openapi.yml
- filename: figure-technology-solutions-heloc-application-requests-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions HELOC application requests API
  slug: figure-technology-solutions-heloc-application-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-heloc-application-requests-api-openapi.yml
- filename: figure-technology-solutions-heloc-offers-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions HELOC Offers API
  slug: figure-technology-solutions-heloc-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-heloc-offers-api-openapi.yml
- filename: figure-technology-solutions-loan-originator-requests-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions Loan Originator requests API
  slug: figure-technology-solutions-loan-originator-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-loan-originator-requests-api-openapi.yml
- filename: figure-technology-solutions-loan-tape-v1-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions Loan Tape V1 API
  slug: figure-technology-solutions-loan-tape-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-loan-tape-v1-api-openapi.yml
- filename: figure-technology-solutions-loan-tape-v2-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions Loan Tape V2 API
  slug: figure-technology-solutions-loan-tape-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-loan-tape-v2-api-openapi.yml
- filename: figure-technology-solutions-payment-history-v1-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions Payment History V1 API
  slug: figure-technology-solutions-payment-history-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-payment-history-v1-api-openapi.yml
- filename: figure-technology-solutions-payment-history-v2-api-openapi.yml
  format: yaml
  label: Figure Technology Solutions Payment History V2 API
  slug: figure-technology-solutions-payment-history-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/openapi/figure-technology-solutions-payment-history-v2-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Figure Technology Solutions Authentication
name_suffix: Authentication
oauth_flows: []
overview: Figure Technology Solutions secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Figure Technology Solutions
provider_slug: figure-technology-solutions
scheme_count: 2
schemes:
- docs: https://docs.figure.com/getting-started
  in: header
  name: apikey
  parameter: apikey
  sources:
  - openapi/figure-technology-solutions-heloc-inquiries-openapi.yml
  type: apiKey
- in: parameter
  name: affiliateId
  note: HELOC Pre-Qualification uses an affiliateId key (not declared as an OpenAPI securityScheme). Sandbox affiliateIds are published in the docs — see sandbox/.
  parameter: affiliateId
  sources:
  - https://docs.figure.com/heloc-pre-qualification/api
  type: apiKey
slug: figure-technology-solutions-authentication
source_filename: figure-technology-solutions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/figure-technology-solutions-heloc-inquiries-openapi.yml\ndocs: https://docs.figure.com/getting-started\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    Every Figure Partner API request requires two headers: an `apikey` header\n    carrying the key Figure supplies to the partner, and a `User-Agent` header.\n    Requests without both headers are rejected. The Portfolio Manager and HELOC\n    Inquiries APIs declare/document the `apikey` header scheme; the HELOC\n    Pre-Qualification API is keyed by an `affiliateId` supplied by Figure.\n    Request/response payloads carrying PII may additionally be JWE-encrypted\n    (RSA-OAEP-256 + A256GCM) — see conventions/ and security docs.\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/figure-technology-solutions-heloc-inquiries-openapi.yml\n  docs: https://docs.figure.com/getting-started\n- name:\
  \ affiliateId\n  type: apiKey\n  in: parameter\n  parameter: affiliateId\n  note: >-\n    HELOC Pre-Qualification uses an affiliateId key (not declared as an OpenAPI\n    securityScheme). Sandbox affiliateIds are published in the docs — see sandbox/.\n  sources:\n  - https://docs.figure.com/heloc-pre-qualification/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/figure-technology-solutions/refs/heads/main/authentication/figure-technology-solutions-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Fintech
- Lending
- HELOC
- Home Equity
- Mortgage
- Capital Markets
- Blockchain
- Loan Origination
- Financial Services
---
