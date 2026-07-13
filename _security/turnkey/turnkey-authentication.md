---
api_key_in:
- header
api_specs:
- filename: turnkey-openapi.yml
  format: yaml
  label: Turnkey Organizations & Sub-Organizations API
  slug: turnkey-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turnkey/refs/heads/main/openapi/turnkey-openapi.yml
- filename: turnkey-openapi.yml
  format: yaml
  label: Turnkey Wallets API
  slug: turnkey-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turnkey/refs/heads/main/openapi/turnkey-openapi.yml
- filename: turnkey-openapi.yml
  format: yaml
  label: Turnkey Private Keys API
  slug: turnkey-private-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turnkey/refs/heads/main/openapi/turnkey-openapi.yml
- filename: turnkey-openapi.yml
  format: yaml
  label: Turnkey Signing & Activities API
  slug: turnkey-signing-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turnkey/refs/heads/main/openapi/turnkey-openapi.yml
- filename: turnkey-openapi.yml
  format: yaml
  label: Turnkey Users, Policies & Authenticators API
  slug: turnkey-users-policies-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turnkey/refs/heads/main/openapi/turnkey-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Turnkey Authentication
name_suffix: Authentication
oauth_flows: []
overview: Turnkey secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Turnkey
provider_slug: turnkey
scheme_count: 2
schemes:
- description: Base64URL-encoded JSON stamp `{publicKey, signature, scheme}` where `signature` is a DER-encoded, hex-encoded signature over the exact JSON POST body produced by the registered API key. `scheme` is one of SIGNATURE_SCHEME_TK_API_P256, SIGNATURE_SCHEME_TK_API_SECP256K1, SIGNATURE_SCHEME_TK_API_ED25519, or SIGNATURE_SCHEME_TK_API_SECP256K1_EIP191. Passkey-stamped requests use the alternate `X-Stamp-
  in: header
  name: apiStamp
  parameter: X-Stamp
  sources:
  - openapi/turnkey-openapi.yml
  type: apiKey
- description: Plain-JSON WebAuthn assertion stamp for passkey-authenticated requests.
  in: header
  name: webauthnStamp
  parameter: X-Stamp-Webauthn
  sources:
  - openapi/turnkey-openapi.yml
  type: apiKey
slug: turnkey-authentication
source_filename: turnkey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/turnkey-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiStamp\n  type: apiKey\n  in: header\n  parameter: X-Stamp\n  description: Base64URL-encoded JSON stamp `{publicKey, signature, scheme}` where `signature`\n    is a DER-encoded, hex-encoded signature over the exact JSON POST body produced by the registered\n    API key. `scheme` is one of SIGNATURE_SCHEME_TK_API_P256, SIGNATURE_SCHEME_TK_API_SECP256K1,\n    SIGNATURE_SCHEME_TK_API_ED25519, or SIGNATURE_SCHEME_TK_API_SECP256K1_EIP191. Passkey-stamped\n    requests use the alternate `X-Stamp-\n  sources:\n  - openapi/turnkey-openapi.yml\n- name: webauthnStamp\n  type: apiKey\n  in: header\n  parameter: X-Stamp-Webauthn\n  description: Plain-JSON WebAuthn assertion stamp for passkey-authenticated requests.\n  sources:\n  - openapi/turnkey-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turnkey/refs/heads/main/authentication/turnkey-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Crypto
- Wallets
- Key Management
- Signing
- Secure Enclaves
---
