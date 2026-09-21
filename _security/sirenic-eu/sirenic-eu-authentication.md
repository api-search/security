---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: sirenic-eu-openapi.yml
  format: yaml
  label: Sirenic API
  slug: sirenic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirenic-eu/refs/heads/main/openapi/sirenic-eu-openapi.yml
auth_types:
- x402 payment (no credential)
- apiKey
- http bearer
- oauth2 (MCP connector only)
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Sirenic Eu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sirenic secures its APIs with x402 payment (no credential), apiKey, http bearer, and oauth2 (MCP connector only) across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sirenic
provider_slug: sirenic-eu
scheme_count: 4
schemes:
- description: 'Sirenic API key (srn_live_…) paying with prepaid credits (1 credit = 1 EUR, same prices as x402). Credits expire 12 months after purchase; calls are charged first to the credits closest to expiry. Optional: without it, the same routes answer 402 with a signable x402 quote. Insufficient balance → 402 {error: credits_insuffisants} WITHOUT a PAYMENT-REQUIRED header. Get a key at /compte.'
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/sirenic-eu-openapi.yml
  type: apiKey
- description: 'The same srn_live_… API key sent as Authorization: Bearer. A bearer value that is not an srn_ key is ignored (x402 flow unchanged).'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sirenic-eu-openapi.yml
  type: http
- applies_to: https://api.sirenic.eu/mcp/connecteur (MCP over OAuth, for assistants) — not the REST API
  dynamic_client_registration: https://api.sirenic.eu/oauth/enregistrement (RFC 7591) + client_id_metadata_document_supported
  flows:
    authorizationCode:
      authorizationUrl: https://api.sirenic.eu/compte/connecteur
      refreshUrl: https://api.sirenic.eu/oauth/jeton
      scopes:
        mcp: call the data routes on behalf of the account holder
      tokenUrl: https://api.sirenic.eu/oauth/jeton
  name: McpConnectorOAuth
  pkce: S256 required
  sources:
  - well-known/sirenic-eu-oauth-authorization-server.json
  - well-known/sirenic-eu-oauth-protected-resource.json
  type: oauth2
- description: 'x402 v2 (kind resource-server) — discovery document at /.well-known/x402 lists every priced resource with its accepts[] (scheme exact, network eip155:8453, asset USDC 0x8335…2913 or EURC 0x60a3…db42, payTo 0x76A672EEe56D29D475b0715cc03B8C99D70EC8A2, maxTimeoutSeconds 120). Not an authentication scheme in the OpenAPI sense (security: [{}] allows anonymous), but it is the default access rail.'
  in: header
  name: X402Payment
  parameter: PAYMENT-SIGNATURE
  sources:
  - well-known/sirenic-eu-x402.json
  - llms/sirenic-eu-llms.txt
  type: x402
slug: sirenic-eu-authentication
source_filename: sirenic-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/sirenic-eu-openapi.yml securitySchemes, enriched from llms.txt (\"PAY WITH AN API KEY INSTEAD OF\n  x402\"), the RFC 8414/9728 discovery documents and the privacy policy MCP-connector section.\nsummary:\n  types:\n  - x402 payment (no credential)\n  - apiKey\n  - http bearer\n  - oauth2 (MCP connector only)\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: 'Sirenic API key (srn_live_…) paying with prepaid credits (1 credit = 1 EUR, same prices as x402).\n    Credits expire 12 months after purchase; calls are charged first to the credits closest to expiry. Optional:\n    without it, the same routes answer 402 with a signable x402 quote. Insufficient balance → 402 {error: credits_insuffisants}\n    WITHOUT a PAYMENT-REQUIRED header. Get a key at /compte.'\n  sources:\n  - openapi/sirenic-eu-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme:\
  \ bearer\n  description: 'The same srn_live_… API key sent as Authorization: Bearer. A bearer value that is not an srn_ key\n    is ignored (x402 flow unchanged).'\n  sources:\n  - openapi/sirenic-eu-openapi.yml\n- name: McpConnectorOAuth\n  type: oauth2\n  applies_to: https://api.sirenic.eu/mcp/connecteur (MCP over OAuth, for assistants) — not the REST API\n  flows:\n    authorizationCode:\n      authorizationUrl: https://api.sirenic.eu/compte/connecteur\n      tokenUrl: https://api.sirenic.eu/oauth/jeton\n      refreshUrl: https://api.sirenic.eu/oauth/jeton\n      scopes:\n        mcp: call the data routes on behalf of the account holder\n  pkce: S256 required\n  dynamic_client_registration: https://api.sirenic.eu/oauth/enregistrement (RFC 7591) + client_id_metadata_document_supported\n  sources:\n  - well-known/sirenic-eu-oauth-authorization-server.json\n  - well-known/sirenic-eu-oauth-protected-resource.json\n- name: X402Payment\n  type: x402\n  in: header\n  parameter: PAYMENT-SIGNATURE\n\
  \  description: 'x402 v2 (kind resource-server) — discovery document at /.well-known/x402 lists every priced resource\n    with its accepts[] (scheme exact, network eip155:8453, asset USDC 0x8335…2913 or EURC 0x60a3…db42, payTo 0x76A672EEe56D29D475b0715cc03B8C99D70EC8A2,\n    maxTimeoutSeconds 120). Not an authentication scheme in the OpenAPI sense (security: [{}] allows anonymous),\n    but it is the default access rail.'\n  sources:\n  - well-known/sirenic-eu-x402.json\n  - llms/sirenic-eu-llms.txt\ndocs:\n- https://api.sirenic.eu/llms.txt\n- https://api.sirenic.eu/openapi.json\n- https://api.sirenic.eu/.well-known/oauth-authorization-server\n- https://api.sirenic.eu/confidentialite\naccess_model:\n  default: No credential. Any /v1 GET without payment answers 402 with an x402 v2 quote (body + PAYMENT-REQUIRED\n    header); the client signs it (USDC or EURC on Base, eip155:8453) and retries with PAYMENT-SIGNATURE. Non-2xx\n    responses are never settled.\n  api_key: 'X-Api-Key: srn_live_…\
  \ or Authorization: Bearer srn_live_… — prepaid credits (1 credit = 1 EUR, packs\n    10/20/50/100 EUR, valid 12 months, closest-to-expiry spent first). Response carries X-Credits-Charged and X-Credits-Remaining.\n    Insufficient balance → 402 {error: credits_insuffisants} without an x402 quote. A signed x402 payment takes\n    precedence over a key.'\n  free_tier: '150 calls/month on routes priced ≤ $0.05 with a verified account (llms.txt / mcp.json). Free routes\n    need nothing: /v1/suggestions, /v1/reperer, /v1/lecture, /v1/provenance/registres, /v1/demo/entreprise, /preview/…,\n    /healthz.'\n  account_gated: GET /v1/documents/{type}/{id} with type=actes requires an identified account (401 otherwise) since\n    2026-09-19 — legal deeds carry personal data.\n  key_storage: Keys and tokens are stored only as SHA-256 fingerprints; the customer area uses magic-link e-mail\n    login, no password (privacy policy, Sécurité).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sirenic-eu/refs/heads/main/authentication/sirenic-eu-authentication.yml
summary_line: x402 payment (no credential)/apiKey/http bearer/oauth2 (MCP connector only) · 4 schemes
tags:
- Company Data
- Business Registry
- KYB
- Know Your Business
- Sanctions Screening
- Financial Data
- Credit Risk
- VAT Validation
- IBAN Validation
- E-Invoicing
- Public Procurement
- Open Data
- France
- Europe
- x402
- Agentic Commerce
- MCP
- A2A
- Company
---
