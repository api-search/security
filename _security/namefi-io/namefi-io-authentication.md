---
anonymous_access: false
api_key_in: []
api_specs:
- filename: namefi-io-admin-api-openapi.yml
  format: yaml
  label: Namefi Admin API
  slug: namefi-io-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-admin-api-openapi.yml
- filename: namefi-io-auth-api-openapi.yml
  format: yaml
  label: Namefi Auth API
  slug: namefi-io-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-auth-api-openapi.yml
- filename: namefi-io-balance-api-openapi.yml
  format: yaml
  label: Namefi Balance API
  slug: namefi-io-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-balance-api-openapi.yml
- filename: namefi-io-base-route-api-openapi.yml
  format: yaml
  label: Namefi Base Route API
  slug: namefi-io-base-route-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-base-route-api-openapi.yml
- filename: namefi-io-ddns-api-openapi.yml
  format: yaml
  label: Namefi Ddns API
  slug: namefi-io-ddns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-ddns-api-openapi.yml
- filename: namefi-io-dns-api-openapi.yml
  format: yaml
  label: Namefi Dns API
  slug: namefi-io-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-dns-api-openapi.yml
- filename: namefi-io-domain-config-api-openapi.yml
  format: yaml
  label: Namefi Domain Config API
  slug: namefi-io-domain-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-domain-config-api-openapi.yml
- filename: namefi-io-eip712-api-openapi.yml
  format: yaml
  label: Namefi Eip712 API
  slug: namefi-io-eip712-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-eip712-api-openapi.yml
- filename: namefi-io-oauth-api-openapi.yml
  format: yaml
  label: Namefi OAuth API
  slug: namefi-io-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-oauth-api-openapi.yml
- filename: namefi-io-orders-api-openapi.yml
  format: yaml
  label: Namefi Orders API
  slug: namefi-io-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-orders-api-openapi.yml
- filename: namefi-io-outbound-api-openapi.yml
  format: yaml
  label: Namefi Outbound API
  slug: namefi-io-outbound-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-outbound-api-openapi.yml
- filename: namefi-io-search-api-openapi.yml
  format: yaml
  label: Namefi Search API
  slug: namefi-io-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-search-api-openapi.yml
- filename: namefi-io-siwe-api-openapi.yml
  format: yaml
  label: Namefi Siwe API
  slug: namefi-io-siwe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-siwe-api-openapi.yml
- filename: namefi-io-studio-api-openapi.yml
  format: yaml
  label: Namefi Studio API
  slug: namefi-io-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-studio-api-openapi.yml
- filename: namefi-io-user-api-openapi.yml
  format: yaml
  label: Namefi User API
  slug: namefi-io-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-user-api-openapi.yml
auth_types: []
description: Authentication methods for Namefi API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Namefi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Namefi declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Namefi
provider_slug: namefi-io
scheme_count: 3
schemes:
- evidence: The simplest authentication method. Works for all operations including DNS record creation, updates, deletes, domain registration, and parking.
  header: x-api-key
  how_to_obtain: Generate an API key from the API keys management page; the key inherits permissions from the wallet that generated it.
  location: header
  name: API Key
  type: apiKey
- evidence: EIP-712 signs a typed-data envelope per request. The current source of truth for the domain and types is the live helper API.
  header: x-namefi-signer, x-namefi-signature, x-namefi-eip712-type
  how_to_obtain: Obtain the signing domain and types from the live helper endpoints (GET /v-next/eip712/domain, GET /v-next/eip712/types, GET /v-next/eip712/types-for-method) and sign the envelope with an external wallet, then include the signer address, signature, and primary type in the respective headers.
  location: header
  name: EIP-712
  type: other
- evidence: SIWE (EIP-4361) gives you a session token after one ERC-191 personal_sign signature. Use it for protected operations that do not require EIP-712.
  header: x-namefi-siwe-token
  how_to_obtain: 'Follow the SIWE flow: GET /v-next/siwe/allowed-chains, GET /v-next/siwe/nonce, GET /v-next/siwe/message, sign the messageString with personal_sign, POST /v-next/siwe/verify, and reuse the returned token.'
  location: header
  name: SIWE
  type: http-bearer
slug: namefi-io-authentication
source_filename: namefi-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.namefi.io/docs/02-authentication
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.namefi.io/docs/02-authentication\nsources:\n- https://docs.namefi.io/docs/02-authentication\n- https://docs.namefi.io/docs/02b-siwe-authentication\n- https://docs.namefi.io/docs/02a-eip712-signing\n- https://docs.namefi.io/docs/02c-prepare-auth-requests\ndescription: Authentication methods for Namefi API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: The simplest authentication method. Works for all operations including DNS record creation, updates, deletes, domain registration,\n    and parking.\n  location: header\n  header: x-api-key\n  how_to_obtain: Generate an API key from the API keys management page; the key inherits permissions from the wallet that generated it.\n- type: other\n  name: EIP-712\n  evidence: EIP-712 signs a typed-data envelope per request. The current source of truth for the domain and types is the live helper API.\n  location: header\n\
  \  header: x-namefi-signer, x-namefi-signature, x-namefi-eip712-type\n  how_to_obtain: Obtain the signing domain and types from the live helper endpoints (GET /v-next/eip712/domain, GET /v-next/eip712/types, GET\n    /v-next/eip712/types-for-method) and sign the envelope with an external wallet, then include the signer address, signature, and primary type\n    in the respective headers.\n- type: http-bearer\n  name: SIWE\n  evidence: SIWE (EIP-4361) gives you a session token after one ERC-191 personal_sign signature. Use it for protected operations that do not require\n    EIP-712.\n  location: header\n  header: x-namefi-siwe-token\n  how_to_obtain: 'Follow the SIWE flow: GET /v-next/siwe/allowed-chains, GET /v-next/siwe/nonce, GET /v-next/siwe/message, sign the messageString\n    with personal_sign, POST /v-next/siwe/verify, and reuse the returned token.'\ndocs: https://docs.namefi.io/docs/02-authentication\n"
source_yaml_url: https://artifacts.apis.io/namefi-io/authentication/namefi-io-authentication.yml
summary_line: 3 schemes
tags:
- Domain Registrar
- Tokenized Domains
- AI Agents
- On‑chain Domains
---
