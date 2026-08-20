---
api_key_in:
- header
api_specs:
- filename: ibanfirst-clientapi-openapi.yml
  format: yaml
  label: iBanFirst API
  slug: ibanfirst-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanfirst/refs/heads/main/openapi/ibanfirst-clientapi-openapi.yml
auth_types:
- apiKey
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Ibanfirst Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: iBanFirst secures its APIs with apiKey, oauth2, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: iBanFirst
provider_slug: ibanfirst
scheme_count: 3
schemes:
- applied_globally: true
  code_samples_published:
  - python
  - javascript
  - php
  - java
  - go
  credential_issuance: Not self-serve. Per the quickstart, "our Support team will generate API tokens linked to your account"; tokens can be granted per method.
  docs: https://docs.ibanfirst.com/api/clientapi/section/authentication-x-wsse
  fields:
  - description: The username assigned during onboarding.
    name: Username
  - description: A Base64-encoded random hex string (>= 32 hex characters).
    name: Nonce
  - description: 'Current UTC timestamp in ISO 8601: YYYY-MM-DDTHH:MM:SSZ.'
    name: Created
  - description: Base64( SHA-1( nonce_bytes + created_bytes + secret_bytes ) ) - SHA-1 binary digest, then Base64.
    name: PasswordDigest
  header_format: 'X-WSSE: UsernameToken Username="<username>", PasswordDigest="<digest>", Nonce="<nonce_b64>", Created="<timestamp>"'
  in: header
  name: X-WSSE
  observations:
  - The digest uses SHA-1. That is the WSSE UsernameToken profile as originally specified, not a modern HMAC construction, and it is worth noting for a payments API - although the secret never crosses the wire and the token is short-lived.
  - There is no bearer/OAuth option on the REST API and no scope model, so authorization is expressed by which methods a support-issued token is granted rather than by scopes.
  parameter: X-WSSE
  scheme_family: WS-Security UsernameToken (WSSE)
  sources:
  - openapi/ibanfirst-clientapi-openapi.yml
  surface: iBanFirst REST API
  token_lifetime: Stateless; expires after approximately 5 minutes, so the header must be recomputed for every request.
  type: apiKey
- bearer_methods_supported:
  - header
  credential_issuance: iBanFirst issues an "OAuth Client ID" and "OAuth Client Password" that the user enters when adding the connector in Claude.
  docs: https://docs.ibanfirst.com/guides/mcp-connector
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://mcp.ibanfirst.com/authorize
    flow: authorizationCode
    pkce: S256
    scopes: {}
    tokenUrl: https://mcp.ibanfirst.com/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://mcp.ibanfirst.com/
  method: probed
  name: MCP OAuth 2.0
  observations:
  - The authorization-server metadata advertises no scopes_supported, so the MCP surface has no published scope vocabulary. Authorization is all-or-nothing per connected account.
  registration_endpoint: https://mcp.ibanfirst.com/register
  scopes_advertised: none
  sources:
  - well-known/ibanfirst-mcp-oauth-authorization-server.json
  - well-known/ibanfirst-mcp-oauth-protected-resource.json
  surface: iBanFirst MCP Connector (https://mcp.ibanfirst.com/mcp)
  token_endpoint_auth_methods_supported:
  - client_secret_post
  type: oauth2
- docs: https://ibanfirst.com/psd2-api
  method: searched
  name: eIDAS QWAC mutual TLS
  probe_result: An anonymous HTTPS request to the sandbox host fails at the TLS layer (curl exit 56, SSL_read error) rather than returning an HTTP status - consistent with a listener that requires a client certificate. No specification could be retrieved.
  requirement: '"If you are a registered Third-Party Provider (TPP), with a qualified EIDAS QWAC and wish to use iBanFirst API, please contact us at open-api@ibanfirst.com"'
  sandbox: https://open-api-sdbx.ibanfirst.com/Banking/API
  sca: Strong customer authentication is in scope of the PSD2 API per the provider's description (accounts information, payment initiation and secure customer authentication).
  surface: iBanFirst PSD2 XS2A API (AIS/PIS)
  type: mutualTLS
slug: ibanfirst-authentication
source_filename: ibanfirst-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: openapi/ibanfirst-clientapi-openapi.yml\ndocs: https://docs.ibanfirst.com/api/clientapi/section/authentication-x-wsse\nnote: >-\n  Derived mechanically from the OpenAPI securitySchemes (one apiKey scheme, X-WSSE in header)\n  and then upgraded from the provider's own documentation, which publishes the full digest\n  algorithm and code samples. Two further authentication models exist on iBanFirst surfaces the\n  OpenAPI does not describe: OAuth 2.0 on the hosted MCP server (metadata probed live) and\n  eIDAS QWAC mutual TLS on the PSD2 XS2A API.\n\nsummary:\n  types:\n    - apiKey\n    - oauth2\n    - mutualTLS\n  api_key_in:\n    - header\n  oauth2_flows:\n    - authorizationCode\n  surfaces: 3\n\nschemes:\n  - name: X-WSSE\n    type: apiKey\n    in: header\n    parameter: X-WSSE\n    surface: iBanFirst REST API\n    sources:\n      - openapi/ibanfirst-clientapi-openapi.yml\n    docs: https://docs.ibanfirst.com/api/clientapi/section/authentication-x-wsse\n\
  \    scheme_family: WS-Security UsernameToken (WSSE)\n    header_format: >-\n      X-WSSE: UsernameToken Username=\"<username>\", PasswordDigest=\"<digest>\",\n      Nonce=\"<nonce_b64>\", Created=\"<timestamp>\"\n    fields:\n      - name: Username\n        description: The username assigned during onboarding.\n      - name: Nonce\n        description: A Base64-encoded random hex string (>= 32 hex characters).\n      - name: Created\n        description: 'Current UTC timestamp in ISO 8601: YYYY-MM-DDTHH:MM:SSZ.'\n      - name: PasswordDigest\n        description: >-\n          Base64( SHA-1( nonce_bytes + created_bytes + secret_bytes ) ) - SHA-1 binary digest,\n          then Base64.\n    token_lifetime: >-\n      Stateless; expires after approximately 5 minutes, so the header must be recomputed for\n      every request.\n    applied_globally: true\n    credential_issuance: >-\n      Not self-serve. Per the quickstart, \"our Support team will generate API tokens linked to\n      your\
  \ account\"; tokens can be granted per method.\n    code_samples_published: [python, javascript, php, java, go]\n    observations:\n      - >-\n        The digest uses SHA-1. That is the WSSE UsernameToken profile as originally specified,\n        not a modern HMAC construction, and it is worth noting for a payments API - although the\n        secret never crosses the wire and the token is short-lived.\n      - >-\n        There is no bearer/OAuth option on the REST API and no scope model, so authorization is\n        expressed by which methods a support-issued token is granted rather than by scopes.\n\n  - name: MCP OAuth 2.0\n    type: oauth2\n    surface: iBanFirst MCP Connector (https://mcp.ibanfirst.com/mcp)\n    sources:\n      - well-known/ibanfirst-mcp-oauth-authorization-server.json\n      - well-known/ibanfirst-mcp-oauth-protected-resource.json\n    docs: https://docs.ibanfirst.com/guides/mcp-connector\n    method: probed\n    flows:\n      - flow: authorizationCode\n       \
  \ authorizationUrl: https://mcp.ibanfirst.com/authorize\n        tokenUrl: https://mcp.ibanfirst.com/token\n        pkce: S256\n        scopes: {}\n    issuer: https://mcp.ibanfirst.com/\n    registration_endpoint: https://mcp.ibanfirst.com/register\n    dynamic_client_registration: true\n    grant_types_supported: [authorization_code, refresh_token]\n    token_endpoint_auth_methods_supported: [client_secret_post]\n    bearer_methods_supported: [header]\n    scopes_advertised: none\n    credential_issuance: >-\n      iBanFirst issues an \"OAuth Client ID\" and \"OAuth Client Password\" that the user enters when\n      adding the connector in Claude.\n    observations:\n      - >-\n        The authorization-server metadata advertises no scopes_supported, so the MCP surface has\n        no published scope vocabulary. Authorization is all-or-nothing per connected account.\n\n  - name: eIDAS QWAC mutual TLS\n    type: mutualTLS\n    surface: iBanFirst PSD2 XS2A API (AIS/PIS)\n    docs: https://ibanfirst.com/psd2-api\n\
  \    method: searched\n    requirement: >-\n      \"If you are a registered Third-Party Provider (TPP), with a qualified EIDAS QWAC and wish\n      to use iBanFirst API, please contact us at open-api@ibanfirst.com\"\n    sandbox: https://open-api-sdbx.ibanfirst.com/Banking/API\n    probe_result: >-\n      An anonymous HTTPS request to the sandbox host fails at the TLS layer (curl exit 56,\n      SSL_read error) rather than returning an HTTP status - consistent with a listener that\n      requires a client certificate. No specification could be retrieved.\n    sca: >-\n      Strong customer authentication is in scope of the PSD2 API per the provider's description\n      (accounts information, payment initiation and secure customer authentication).\n\nx-evidence:\n  checked: '2026-08-17'\n  probes:\n    - url: https://docs.ibanfirst.com/_spec/api/ClientAPI.yaml\n      http_status: 200\n    - url: https://docs.ibanfirst.com/api/clientapi/section/authentication-x-wsse\n      http_status: 200\n\
  \    - url: https://mcp.ibanfirst.com/.well-known/oauth-authorization-server\n      http_status: 200\n    - url: https://open-api-sdbx.ibanfirst.com/Banking/API\n      http_status: 0\n      note: TLS handshake terminated by the server; no HTTP response\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibanfirst/refs/heads/main/authentication/ibanfirst-authentication.yml
summary_line: apiKey/oauth2/mutualTLS · 3 schemes
tags:
- Company
- Fintech Insurtech
- Cross-Border Payments
- Foreign Exchange
- B2B Payments
- Treasury
- multi-currency-accounts
- Swift
- SEPA
- PSD2
- Open Banking
- currency-risk-management
- Webhook
- MCP
- Belgium
- Europe
---
