---
api_key_in: []
auth_types:
- oauth2
description: Authentication profile for HKEX's one documented RESTful API, the FINI API Gateway (IPO settlement). Access is restricted to registered market participants (HKSCC Participants, FINI banks, sponsors, advisers). Clients authenticate with OAuth 2.0 JWT-bearer grants (RFC 7523) against the HKEX Access Management (ForgeRock OpenAM) server, presenting two RS256-signed JWTs — an Agent Profile JWT (G1) and a Machine Profile JWT (G2) — whose RSA JSON Web Keys (RFC 7517) are pre-registered on the HKEX Access Management Portal. The AM server returns a FINI API JWT access token that is passed as a Bearer token on every FINI API call. The OMD market-data feeds and the Data Marketplace are not HTTP APIs and use licensing agreements / SFTP credentials instead.
kind: authentication
layout: security
method: searched
name: Hkex Authentication
name_suffix: Authentication
oauth_flows:
- jwt-bearer
overview: HKEX secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the jwt-bearer flow(s).
provider_name: HKEX
provider_slug: hkex
scheme_count: 1
schemes:
- assertions:
  - algorithm: RS256
    name: Agent Profile JWT (G1)
    registered_key: Agent RSA JWK registered on HKEX Access Management Portal
    sub: user's Company ID in HKEX Client Connect
  - algorithm: RS256
    name: Machine Profile JWT (G2)
    registered_key: Machine RSA JWK registered on HKEX Access Management Portal
  client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer
  constraints:
  - Agent/Machine Profile JWT expiration must be within 30 minutes or the AM server rejects it
  - Access token expires_in 30 (seconds, per sample response); scope value returned is the Company ID (e.g. CP00001)
  - Registered JWKs expire and must be rotated before expiry
  entitlements:
  - function: EU_finiIPORefDataAPI
    grants: /api/ipos/* (all FINI users)
  - function: EU_finiPOSubAPI
    grants: /api/eipo/subscriptions/* (HKSCC Participants)
  - function: EU_finiPOFundAPI
    grants: /api/eipo/funding/* (EIPO Designated Banks)
  flow: urn:ietf:params:oauth:grant-type:jwt-bearer
  name: FINI OAuth 2.0 JWT-bearer
  token_host: https://openam.connect.hkex.com.hk
  token_path: /openam/oauth2/eu/access_token
  type: oauth2
  usage: 'Send the FINI API JWT access token as "Authorization: Bearer <token>" on every FINI API request'
slug: hkex-authentication
source_filename: hkex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://www.hkex.com.hk/-/media/HKEX-Market/Services/Next-Generation-Post-Trade-Programme/Fini/FINI-API-User-Guide-v0,-d-,41.pdf\ndocs: https://www.hkex.com.hk/Services/Platform-Services/FINI?sc_lang=en\ndescription: >-\n  Authentication profile for HKEX's one documented RESTful API, the FINI API\n  Gateway (IPO settlement). Access is restricted to registered market\n  participants (HKSCC Participants, FINI banks, sponsors, advisers). Clients\n  authenticate with OAuth 2.0 JWT-bearer grants (RFC 7523) against the HKEX\n  Access Management (ForgeRock OpenAM) server, presenting two RS256-signed\n  JWTs — an Agent Profile JWT (G1) and a Machine Profile JWT (G2) — whose RSA\n  JSON Web Keys (RFC 7517) are pre-registered on the HKEX Access Management\n  Portal. The AM server returns a FINI API JWT access token that is passed as\n  a Bearer token on every FINI API call. The OMD market-data feeds and the\n  Data Marketplace are not\
  \ HTTP APIs and use licensing agreements / SFTP\n  credentials instead.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [jwt-bearer]\n  transport: TLS 1.2 minimum; PII request/response fields additionally use end-to-end field-level encryption\nschemes:\n- name: FINI OAuth 2.0 JWT-bearer\n  type: oauth2\n  flow: 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  client_assertion_type: 'urn:ietf:params:oauth:client-assertion-type:jwt-bearer'\n  token_host: https://openam.connect.hkex.com.hk\n  token_path: /openam/oauth2/eu/access_token\n  assertions:\n  - name: Agent Profile JWT (G1)\n    algorithm: RS256\n    sub: user's Company ID in HKEX Client Connect\n    registered_key: Agent RSA JWK registered on HKEX Access Management Portal\n  - name: Machine Profile JWT (G2)\n    algorithm: RS256\n    registered_key: Machine RSA JWK registered on HKEX Access Management Portal\n  constraints:\n  - Agent/Machine Profile JWT expiration must be within 30 minutes or the AM server rejects it\n  - Access\
  \ token expires_in 30 (seconds, per sample response); scope value returned is the Company ID (e.g. CP00001)\n  - Registered JWKs expire and must be rotated before expiry\n  usage: 'Send the FINI API JWT access token as \"Authorization: Bearer <token>\" on every FINI API request'\n  entitlements:\n  - function: EU_finiIPORefDataAPI\n    grants: /api/ipos/* (all FINI users)\n  - function: EU_finiPOSubAPI\n    grants: /api/eipo/subscriptions/* (HKSCC Participants)\n  - function: EU_finiPOFundAPI\n    grants: /api/eipo/funding/* (EIPO Designated Banks)\nnotes:\n- No self-serve signup — credentials are provisioned through HKEX Client Connect / Access Management for registered participants only.\n- The OpenAM host is not reachable from the public internet; OIDC discovery could not be probed anonymously.\n- OMD-C / OMD-D datafeeds are licensed binary multicast feeds (no HTTP authentication surface); Data Marketplace delivery uses SFTP or cloud-to-cloud transfer arranged with the datamarketplace@hkex.com.hk\
  \ team.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hkex/refs/heads/main/authentication/hkex-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Financial
- Market Data
- Stocks
- Derivatives
- Exchange
- Real-Time
- Historical Data
- Order Book
- Reference Data
- IPO
---
