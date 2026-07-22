---
api_key_in:
- header
api_specs:
- filename: stark-bank-openapi-original.yml
  format: yaml
  label: Stark Bank API
  slug: stark-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stark-bank/refs/heads/main/openapi/stark-bank-openapi-original.yml
auth_types:
- digitalSignature
description: ''
kind: authentication
layout: security
method: searched
name: Stark Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stark Bank secures its APIs with digitalSignature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stark Bank
provider_slug: stark-bank
scheme_count: 1
schemes:
- curve: secp256k1
  description: ECDSA digital signature (secp256k1, SHA-256) for request authentication. Requests carry Access-Id (project/organization/workspace id), Access-Time (unix timestamp) and Access-Signature (base64 ECDSA signature) headers; webhook event bodies are verified with the same scheme via the Digital-Signature header. The official SDKs sign and verify automatically.
  digest: sha-256
  in: header
  name: digitalSignature
  parameter: Digital-Signature
  sources:
  - openapi/stark-bank-openapi-original.yml
  type: apiKey
  user_types:
  - project
  - organization
slug: stark-bank-authentication
source_filename: stark-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/stark-bank-openapi-original.yml\ndocs: https://docs.starkbank.com/how-to-create-ecdsa-keys\nsummary:\n  types:\n  - digitalSignature\n  api_key_in:\n  - header\n  model: ecdsa-request-signing\n  notes: >-\n    Stark Bank does not use static API keys or OAuth. Every request is signed\n    locally with an ECDSA private key (secp256k1 curve, SHA-256 digest) and\n    verified server-side against the public key registered in Web Banking. The\n    OpenAPI models this as a single apiKey-style header scheme (digitalSignature).\nschemes:\n- name: digitalSignature\n  type: apiKey\n  in: header\n  parameter: Digital-Signature\n  description: >-\n    ECDSA digital signature (secp256k1, SHA-256) for request authentication.\n    Requests carry Access-Id (project/organization/workspace id), Access-Time\n    (unix timestamp) and Access-Signature (base64 ECDSA signature) headers;\n    webhook event bodies are verified with the same\
  \ scheme via the\n    Digital-Signature header. The official SDKs sign and verify automatically.\n  curve: secp256k1\n  digest: sha-256\n  user_types:\n  - project\n  - organization\n  sources:\n  - openapi/stark-bank-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stark-bank/refs/heads/main/authentication/stark-bank-authentication.yml
summary_line: digitalSignature · 1 scheme
tags:
- Company
- Fintech
- Banking
- Payments
- Pix
- Boleto
- Banking as a Service
- Brazil
- Financial Services
---
