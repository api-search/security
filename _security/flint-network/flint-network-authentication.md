---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: flint-network-agent-passport-api-openapi.yml
  format: yaml
  label: FLINT Network Agent Passport API
  slug: flint-network-agent-passport-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flint-network/openapi/flint-network-agent-passport-api-openapi.yml
- filename: flint-network-agent-sessions-api-openapi.yml
  format: yaml
  label: FLINT Network Agent Sessions API
  slug: flint-network-agent-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flint-network/openapi/flint-network-agent-sessions-api-openapi.yml
- filename: flint-network-outcome-feedback-api-openapi.yml
  format: yaml
  label: FLINT Network Outcome Feedback API
  slug: flint-network-outcome-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flint-network/openapi/flint-network-outcome-feedback-api-openapi.yml
- filename: flint-network-scout-credits-api-openapi.yml
  format: yaml
  label: FLINT Network Scout Credits API
  slug: flint-network-scout-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flint-network/openapi/flint-network-scout-credits-api-openapi.yml
- filename: flint-network-trust-graph-api-openapi.yml
  format: yaml
  label: FLINT Network Trust Graph API
  slug: flint-network-trust-graph-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flint-network/openapi/flint-network-trust-graph-api-openapi.yml
- filename: flint-network-verification-records-api-openapi.yml
  format: yaml
  label: FLINT Network Verification Records API
  slug: flint-network-verification-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flint-network/openapi/flint-network-verification-records-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 6
method: derived
name: FLINT Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: FLINT Network secures its APIs with apiKey and http across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FLINT Network
provider_slug: flint-network
scheme_count: 6
schemes:
- description: Sealed WorkOS session required for claimed-Passport owner actions. Unclaimed mandate updates require the claim token as a management capability.
  in: cookie
  name: WorkOSOwnerSession
  parameter: flint_session
  sources:
  - openapi/flint-network-openapi.json
  type: apiKey
- description: Server-only partner credential. The authenticated partner must match the partner in the stored signed verification record.
  name: PartnerServiceBearer
  scheme: bearer
  sources:
  - openapi/flint-network-openapi.json
  type: http
- description: Canonical x402 v2 payment proof on a paid retry. Initial unpaid challenge requests require no payment proof.
  in: header
  name: X402Payment
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/flint-network-openapi.json
  type: apiKey
- description: Short-lived Passport-owner-issued capability bound to the exact x402 Verify request.
  in: header
  name: FlintCapability
  parameter: FLINT-CAPABILITY
  sources:
  - openapi/flint-network-openapi.json
  type: apiKey
- description: Fresh caller proof bound to the capability, request, and x402 payment proof.
  in: header
  name: DPoP
  parameter: DPoP
  sources:
  - openapi/flint-network-openapi.json
  type: apiKey
- description: Base64url-encoded x401 principal-identity presentation. Omit to request a proof challenge.
  in: header
  name: X401Proof
  parameter: PROOF-RESPONSE
  sources:
  - openapi/flint-network-openapi.json
  type: apiKey
slug: flint-network-authentication
source_filename: flint-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/flint-network-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: WorkOSOwnerSession\n  type: apiKey\n  in: cookie\n  parameter: flint_session\n  description: Sealed WorkOS session required for claimed-Passport owner actions. Unclaimed\n    mandate updates require the claim token as a management capability.\n  sources:\n  - openapi/flint-network-openapi.json\n- name: PartnerServiceBearer\n  type: http\n  scheme: bearer\n  description: Server-only partner credential. The authenticated partner must match the partner\n    in the stored signed verification record.\n  sources:\n  - openapi/flint-network-openapi.json\n- name: X402Payment\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: Canonical x402 v2 payment proof on a paid retry. Initial unpaid challenge requests\n    require no payment proof.\n  sources:\n  - openapi/flint-network-openapi.json\n\
  - name: FlintCapability\n  type: apiKey\n  in: header\n  parameter: FLINT-CAPABILITY\n  description: Short-lived Passport-owner-issued capability bound to the exact x402 Verify request.\n  sources:\n  - openapi/flint-network-openapi.json\n- name: DPoP\n  type: apiKey\n  in: header\n  parameter: DPoP\n  description: Fresh caller proof bound to the capability, request, and x402 payment proof.\n  sources:\n  - openapi/flint-network-openapi.json\n- name: X401Proof\n  type: apiKey\n  in: header\n  parameter: PROOF-RESPONSE\n  description: Base64url-encoded x401 principal-identity presentation. Omit to request a proof\n    challenge.\n  sources:\n  - openapi/flint-network-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/flint-network/authentication/flint-network-authentication.yml
summary_line: apiKey/http · 6 schemes
tags:
- Artificial Intelligence
- Fraud Prevention
- Compliance
- Agentic Commerce
- Real-Time
---
