---
api_key_in:
- header
auth_types:
- mutualTLS
- apiKey
- requestSignature
description: ''
kind: authentication
layout: security
method: searched
name: Shieldpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shieldpay secures its APIs with mutualTLS, apiKey, and requestSignature across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Shieldpay
provider_slug: shieldpay
scheme_count: 4
schemes:
- description: Client and server verify each other with certificates over an encrypted mTLS channel. The integrator generates a Private Key and CSR; Shieldpay issues one Signed Certificate per organisation at a time. Certificate lifecycle requests go to integrationsupport@shieldpay.com.
  name: mutualTLS
  type: mutualTLS
- description: A unique secret token identifying the organisation, sent in the Authorization header of every request. API keys do not expire but can be deactivated; an organisation may hold multiple active keys. Registration/deactivation via integrationsupport@shieldpay.com.
  in: header
  name: apiKey
  parameter_name: Authorization
  type: apiKey
- algorithm: RSA-SHA256
  description: 'Every request must carry a DigitalSignature header. The signature is an RSA-SHA256 signature (Base64) over the concatenation, in order and with no separators, of: Request URL (no query string) + API Key + RequestID + Timestamp + raw Request Body, signed with the client Private Key.'
  name: requestSignature
  parameter_name: DigitalSignature
  scheme: signature
  type: http
- description: All requests must originate from a whitelisted IP. Sandbox and Production maintain separate whitelists. Changes via integrationsupport@shieldpay.com, actioned within hours to two UK business days.
  name: ipWhitelist
  type: networkControl
slug: shieldpay-authentication
source_filename: shieldpay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.shieldpay.com/getting-started/api-fundamentals/authentication-and-security\ndocs: https://developers.shieldpay.com/getting-started/api-fundamentals/authentication-and-security/authentication-mtls-and-api-keys\nsummary:\n  types: [mutualTLS, apiKey, requestSignature]\n  api_key_in: [header]\n  api_key_header: Authorization\n  transport_security: mutual-TLS\n  oauth2_flows: []\n  note: >-\n    No OAuth2/OIDC. Access is layered: mutual TLS establishes the channel, an API\n    key identifies the organisation, and every request is signed and IP-gated.\nschemes:\n- name: mutualTLS\n  type: mutualTLS\n  description: >-\n    Client and server verify each other with certificates over an encrypted mTLS\n    channel. The integrator generates a Private Key and CSR; Shieldpay issues one\n    Signed Certificate per organisation at a time. Certificate lifecycle requests\n    go to integrationsupport@shieldpay.com.\n- name:\
  \ apiKey\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  description: >-\n    A unique secret token identifying the organisation, sent in the Authorization\n    header of every request. API keys do not expire but can be deactivated; an\n    organisation may hold multiple active keys. Registration/deactivation via\n    integrationsupport@shieldpay.com.\n- name: requestSignature\n  type: http\n  scheme: signature\n  parameter_name: DigitalSignature\n  algorithm: RSA-SHA256\n  description: >-\n    Every request must carry a DigitalSignature header. The signature is an\n    RSA-SHA256 signature (Base64) over the concatenation, in order and with no\n    separators, of: Request URL (no query string) + API Key + RequestID +\n    Timestamp + raw Request Body, signed with the client Private Key.\n- name: ipWhitelist\n  type: networkControl\n  description: >-\n    All requests must originate from a whitelisted IP. Sandbox and Production\n    maintain separate whitelists. Changes\
  \ via integrationsupport@shieldpay.com,\n    actioned within hours to two UK business days.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shieldpay/refs/heads/main/authentication/shieldpay-authentication.yml
summary_line: mutualTLS/apiKey/requestSignature · 4 schemes
tags:
- Company
- Payments
- Escrow
- Legal Technology
- Fintech
- Compliance
- KYC
- Banking
---
