---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coudrebros-eu-auth-api-openapi.yml
  format: yaml
  label: Coudre Bros. Auth API
  slug: coudrebros-eu-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coudrebros-eu/openapi/coudrebros-eu-auth-api-openapi.yml
- filename: coudrebros-eu-health-api-openapi.yml
  format: yaml
  label: Coudre Bros. Health API
  slug: coudrebros-eu-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coudrebros-eu/openapi/coudrebros-eu-health-api-openapi.yml
- filename: coudrebros-eu-mint-api-openapi.yml
  format: yaml
  label: Coudre Bros. Mint API
  slug: coudrebros-eu-mint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coudrebros-eu/openapi/coudrebros-eu-mint-api-openapi.yml
- filename: coudrebros-eu-notary-api-openapi.yml
  format: yaml
  label: Coudre Bros. Notary API
  slug: coudrebros-eu-notary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coudrebros-eu/openapi/coudrebros-eu-notary-api-openapi.yml
- filename: coudrebros-eu-payment-api-openapi.yml
  format: yaml
  label: Coudre Bros. Payment API
  slug: coudrebros-eu-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coudrebros-eu/openapi/coudrebros-eu-payment-api-openapi.yml
- filename: coudrebros-eu-prerequisites-api-openapi.yml
  format: yaml
  label: Coudre Bros. Prerequisites API
  slug: coudrebros-eu-prerequisites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coudrebros-eu/openapi/coudrebros-eu-prerequisites-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Coudre Bros. Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coudre Bros. secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coudre Bros.
provider_slug: coudrebros-eu
scheme_count: 1
schemes:
- declared_in_spec: false
  description: 'Send the key as `Authorization: Bearer <key>` on every request below.'
  expiry: 'Privacy policy at https://www.coudrebros.eu/nft_api/#legal: keys are kept indefinitely until manually revoked by the operator; there is currently no automatic expiration.'
  header: Authorization
  in: header
  issuance: POST /register (register_register_post) -- pay a one-time 3 ADA registration fee from the Cardano address the key is bound to, then call /register with that transaction hash; no manual sign-up. One active API key per address; the key is shown once.
  name: bearerApiKey
  revocation: Registering again with an already-registered address is rejected -- ask the operator to revoke the old key first if you need a new one.
  scheme: bearer
  type: http
slug: coudrebros-eu-authentication
source_filename: coudrebros-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://nftapi.coudrebros.eu/openapi.json\ndocs: https://nftapi.coudrebros.eu/docs#/auth\nsummary:\n  types:\n  - http\n  note: The OpenAPI declares no components.securitySchemes; auth is documented in info.description and modelled as an `authorization` header parameter on each protected operation.\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: 'Send the key as `Authorization: Bearer <key>` on every request below.'\n  issuance: POST /register (register_register_post) -- pay a one-time 3 ADA registration fee from the Cardano address the key is bound to, then call /register with that transaction hash; no manual sign-up. One active API key per address; the key is shown once.\n  revocation: 'Registering again with an already-registered address is rejected -- ask the operator to revoke the old key first if you need a new one.'\n  expiry: 'Privacy policy at https://www.coudrebros.eu/nft_api/#legal:\
  \ keys are kept indefinitely until manually revoked by the operator; there is currently no automatic expiration.'\n  declared_in_spec: false\nunauthenticated_operations:\n- info_info_get\n- notary_info_notary_info_get\n- verify_proof_notary_verify_post\n- verify_decision_chain_notary_decision_verify_post\n- health_health_get\n- register_register_post\nmcp_note: 'The MCP endpoint (https://nftapi.coudrebros.eu/mcp) has no OAuth or sign-in step -- authentication is a per-call api_key tool argument (stated on https://www.coudrebros.eu/nft_api/).'\n"
source_yaml_url: https://artifacts.apis.io/coudrebros-eu/authentication/coudrebros-eu-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cardano
- Blockchain
- Stake Pool
- NFT
- Minting
- Notary
- AI Agents
- MCP
- Web3
---
