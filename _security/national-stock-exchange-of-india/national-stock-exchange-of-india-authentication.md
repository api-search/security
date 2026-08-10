---
api_key_in:
- header
auth_types:
- http
- apiKey
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: National Stock Exchange Of India Authentication
name_suffix: Authentication
oauth_flows: []
overview: National Stock Exchange of India secures its APIs with http, apiKey, and mutualTLS across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: National Stock Exchange of India
provider_slug: national-stock-exchange-of-india
scheme_count: 5
schemes:
- api: NSE RFQ Web API
  description: POST /rest/v1/login exchanges member credentials for a session token; the token is sent on every subsequent call in the `loginKey` header. A second login with the same credentials expires the older session, and an idle session expires after a fixed interval (HTTP 401).
  in: header
  name: rfq-login-session
  parameter_name: loginKey
  source: RFQ - Protocol for Web API v1.1.10 (PDF), "General Instructions" and "Login API"
  type: apiKey
- api: NSE RFQ Web API (callbacks)
  description: Outbound RFQ notification callbacks are authenticated to the participant by an HMAC-SHA256 of the request JSON payload, hex-encoded and sent in the `token` header. The participant callback base URL must be HTTPS and is registered with the Exchange.
  in: header
  name: rfq-callback-signature
  parameter_name: token
  source: RFQ - Protocol for Web API v1.1.10 (PDF), "Callbacks API"
  type: apiKey
- api: NSE Offer For Sale (OFS) Web API
  description: POST /auth/token issues an accessToken for valid member credentials; POST /auth/refreshToken renews it. The token value is sent in the `Authorization` header on every call except the login API.
  in: header
  name: ofs-access-token
  parameter_name: Authorization
  scheme: bearer
  source: OFS-WEB API v1.3.4 (PDF), "General Instructions" / "POST /auth/token"
  type: http
- api: NSE RFQ FIX Interface (FIX 5.0 SP2 / FIXT.1.1)
  description: The FIX gateway session is encrypted with SSL/TLS and client certificate authentication is enabled — participant applications must present a valid certificate during the SSL handshake, in addition to the FIX Logon (A) message credentials.
  name: nse-rfq-fix-mtls
  source: NSE RFQ - FIX Interface Protocol v1.0.2 (PDF), "Connection & Session Management"
  type: mutualTLS
- api: Non-NEAT Front-End (NNF) trading protocol
  description: The binary NNF / Drop Copy / MTBT trading protocols authenticate with Exchange-issued member user IDs over dedicated connectivity (leased line, colocation, extranet). Not an HTTP scheme.
  name: nnf-member-credentials
  source: NSE Trading Protocols page (PDF/ZIP protocol documents)
  type: proprietary
slug: national-stock-exchange-of-india-authentication
source_filename: national-stock-exchange-of-india-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: NSE trading protocol documents (PDF) published at https://www.nseindia.com/static/trade/platform-services-neat-trading-system-protocols\ndocs: https://www.nseindia.com/static/trade/platform-services-neat-trading-system-protocols\nnote: >-\n  NSE publishes no OpenAPI, so no securityScheme could be derived. Every scheme below was read\n  directly out of NSE's own published protocol PDFs. All NSE interfaces are member/participant\n  interfaces: credentials are issued by the Exchange to an enabled member user, there is no\n  self-service sign-up and there is no OAuth 2.0 or OpenID Connect anywhere in the surface.\nsummary:\n  types: [http, apiKey, mutualTLS]\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\n  oidc: false\n  self_service_signup: false\nschemes:\n- name: rfq-login-session\n  api: NSE RFQ Web API\n  type: apiKey\n  in: header\n  parameter_name: loginKey\n  description: >-\n    POST /rest/v1/login exchanges\
  \ member credentials for a session token; the token is sent on\n    every subsequent call in the `loginKey` header. A second login with the same credentials\n    expires the older session, and an idle session expires after a fixed interval (HTTP 401).\n  source: RFQ - Protocol for Web API v1.1.10 (PDF), \"General Instructions\" and \"Login API\"\n- name: rfq-callback-signature\n  api: NSE RFQ Web API (callbacks)\n  type: apiKey\n  in: header\n  parameter_name: token\n  description: >-\n    Outbound RFQ notification callbacks are authenticated to the participant by an HMAC-SHA256\n    of the request JSON payload, hex-encoded and sent in the `token` header. The participant\n    callback base URL must be HTTPS and is registered with the Exchange.\n  source: RFQ - Protocol for Web API v1.1.10 (PDF), \"Callbacks API\"\n- name: ofs-access-token\n  api: NSE Offer For Sale (OFS) Web API\n  type: http\n  scheme: bearer\n  in: header\n  parameter_name: Authorization\n  description: >-\n    POST\
  \ /auth/token issues an accessToken for valid member credentials; POST /auth/refreshToken\n    renews it. The token value is sent in the `Authorization` header on every call except the\n    login API.\n  source: OFS-WEB API v1.3.4 (PDF), \"General Instructions\" / \"POST /auth/token\"\n- name: nse-rfq-fix-mtls\n  api: NSE RFQ FIX Interface (FIX 5.0 SP2 / FIXT.1.1)\n  type: mutualTLS\n  description: >-\n    The FIX gateway session is encrypted with SSL/TLS and client certificate authentication is\n    enabled — participant applications must present a valid certificate during the SSL handshake,\n    in addition to the FIX Logon (A) message credentials.\n  source: NSE RFQ - FIX Interface Protocol v1.0.2 (PDF), \"Connection & Session Management\"\n- name: nnf-member-credentials\n  api: Non-NEAT Front-End (NNF) trading protocol\n  type: proprietary\n  description: >-\n    The binary NNF / Drop Copy / MTBT trading protocols authenticate with Exchange-issued member\n    user IDs over dedicated\
  \ connectivity (leased line, colocation, extranet). Not an HTTP scheme.\n  source: NSE Trading Protocols page (PDF/ZIP protocol documents)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-stock-exchange-of-india/refs/heads/main/authentication/national-stock-exchange-of-india-authentication.yml
summary_line: http/apiKey/mutualTLS · 5 schemes
tags:
- Company
- Stock Exchange
- Capital Markets
- Market Data
- Trading
- Financial Services
- Securities
- India
- FIX Protocol
- Bonds
---
