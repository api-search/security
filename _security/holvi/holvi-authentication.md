---
api_key_in:
- header
api_specs:
- filename: holvi-psd2-openapi.yml
  format: yaml
  label: Holvi PSD2 API
  slug: holvi-psd2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holvi/refs/heads/main/openapi/holvi-psd2-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Holvi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Holvi secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Holvi
provider_slug: holvi
scheme_count: 4
schemes:
- description: Client ID identifying the TPP application (from approved onboarding).
  in: header
  name: HolviClientId
  parameter: X-Holvi-Client-Id
  sources:
  - openapi/holvi-psd2-openapi.yml
  type: apiKey
- description: Client Secret authenticating the TPP (from approved onboarding).
  in: header
  name: HolviClientSecret
  parameter: X-Holvi-Client-Secret
  sources:
  - openapi/holvi-psd2-openapi.yml
  type: apiKey
- description: Application-level HTTP message signature (Draft Cavage HTTP Signatures v10, RSA-SHA256, key >= 2048-bit) over (request-target), Host, Date [, Content-Type, Digest for write methods], keyId = Client-Id, using the eIDAS QSEAL certificate.
  in: header
  name: HolviSignatureHeader
  parameter: Signature
  sources:
  - openapi/holvi-psd2-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: PSU consent JWT access token from the consent token exchange.
  name: HolviBearer
  scheme: bearer
  sources:
  - openapi/holvi-psd2-openapi.yml
  type: http
slug: holvi-authentication
source_filename: holvi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/holvi-psd2-openapi.yml\ndocs: https://holvi.github.io/psd2-api/authentication.html\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  model: >-\n    Two-party authentication. The TPP proves itself with an eIDAS QSEAL client certificate,\n    a Holvi Client-Id/Client-Secret pair, and a per-request HTTP message signature (Draft\n    Cavage HTTP Signatures v10, RSA-SHA256, key >= 2048-bit) over (request-target), Host,\n    Date and, for write methods, Content-Type and Digest (RFC 3230 SHA-256). The end user\n    (PSU) grants consent via a redirect login at https://psd2.holvi.com/login/ and the\n    returned authorization code is exchanged for a JWT bearer access token used in the\n    Authorization header. Onboarding endpoints are exempt from the signature requirement.\nschemes:\n- name: HolviClientId\n  type: apiKey\n  in: header\n  parameter: X-Holvi-Client-Id\n  description: Client ID identifying\
  \ the TPP application (from approved onboarding).\n  sources:\n  - openapi/holvi-psd2-openapi.yml\n- name: HolviClientSecret\n  type: apiKey\n  in: header\n  parameter: X-Holvi-Client-Secret\n  description: Client Secret authenticating the TPP (from approved onboarding).\n  sources:\n  - openapi/holvi-psd2-openapi.yml\n- name: HolviSignatureHeader\n  type: apiKey\n  in: header\n  parameter: Signature\n  description: Application-level HTTP message signature (Draft Cavage HTTP Signatures v10, RSA-SHA256,\n    key >= 2048-bit) over (request-target), Host, Date [, Content-Type, Digest for write methods],\n    keyId = Client-Id, using the eIDAS QSEAL certificate.\n  sources:\n  - openapi/holvi-psd2-openapi.yml\n- name: HolviBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: PSU consent JWT access token from the consent token exchange.\n  sources:\n  - openapi/holvi-psd2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holvi/refs/heads/main/authentication/holvi-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Banking
- Fintech
- Payments
- Business Banking
- PSD2
- Open Banking
- SEPA
- Finland
---
