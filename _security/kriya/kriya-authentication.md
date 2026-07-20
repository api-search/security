---
api_key_in:
- header
api_specs:
- filename: kriya-payments-openapi.yaml
  format: yaml
  label: Kriya Payments API
  slug: kriya-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya/refs/heads/main/openapi/kriya-payments-openapi.yaml
- filename: kriya-onboarding-openapi.yaml
  format: yaml
  label: Kriya Onboarding API
  slug: kriya-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya/refs/heads/main/openapi/kriya-onboarding-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Kriya Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kriya secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kriya
provider_slug: kriya
scheme_count: 1
schemes:
- applies_to:
  - openapi/kriya-payments-openapi.yaml
  - openapi/kriya-onboarding-openapi.yaml
  declared_in_spec: false
  description: Partner API key issued by Kriya on approval. Must be sent with every request to both the Payments API and the Onboarding API. Separate keys are issued per environment (Test and Production) and must be requested separately.
  in: header
  name: X-Kriya-ApiKey
  parameter_name: X-Kriya-ApiKey
  source: https://docs.kriya.co/payments#section/Introduction/Authorization
  type: apiKey
slug: kriya-authentication
source_filename: kriya-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.kriya.co/payments#section/Introduction/Authorization\ndocs: https://docs.kriya.co/payments#section/Introduction/Authorization\nnote: >-\n  Neither published OpenAPI document declares components.securitySchemes, so the\n  mechanical derive pass (0-working/derive-authentication.py) produced no profile.\n  This profile is captured from the Authorization section of the Kriya Payments API\n  documentation, which the Onboarding API explicitly reuses. Recording the spec gap\n  is deliberate: the auth model is real and documented in prose, but absent from the\n  machine-readable contract.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: X-Kriya-ApiKey\n  type: apiKey\n  in: header\n  parameter_name: X-Kriya-ApiKey\n  description: >-\n    Partner API key issued by Kriya on approval. Must be sent with every request to\n    both the Payments API and the Onboarding API. Separate\
  \ keys are issued per\n    environment (Test and Production) and must be requested separately.\n  applies_to:\n  - openapi/kriya-payments-openapi.yaml\n  - openapi/kriya-onboarding-openapi.yaml\n  declared_in_spec: false\n  source: https://docs.kriya.co/payments#section/Introduction/Authorization\nwebhook_verification:\n- name: X-Kriya-Signature\n  type: hmac\n  algorithm: HMAC-SHA256\n  encoding: base64\n  direction: inbound-to-partner\n  description: >-\n    Kriya signs each outbound webhook payload with a partner-specific HMAC key and\n    sends the base64-encoded HMAC-SHA256 digest in the X-Kriya-Signature request\n    header. Partners verify by recomputing the digest over the raw payload and\n    comparing values.\n  source: https://docs.kriya.co/payments#section/Webhooks/Verifying-Webhooks\naccess_model:\n  provisioning: >-\n    Access is restricted to approved partners; API keys and the webhook HMAC key are\n    issued by the Kriya team during merchant onboarding.\n  environments:\n\
  \  - name: Test\n    base_urls:\n    - https://api.kriya.dev/payments/\n    - https://api.kriya.dev/onboarding/\n  - name: Production\n    base_urls:\n    - https://api.kriya.co/payments/\n    - https://api.kriya.co/onboarding/\n  transport: All API requests must be sent over HTTPS.\n  oauth2: false\n  scopes: false\ncontact: apisupport@kriya.co\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kriya/refs/heads/main/authentication/kriya-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Payments
- Embedded Finance
- Buy Now Pay Later
- B2B Payments
- Invoice Finance
- Lending
- Working Capital
- Onboarding
- KYC
- United Kingdom
---
