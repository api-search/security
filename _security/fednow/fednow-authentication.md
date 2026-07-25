---
api_key_in:
- header
auth_types:
- mutualTLS
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Fednow Authentication
name_suffix: Authentication
oauth_flows: []
overview: FedNow Service secures its APIs with mutualTLS and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FedNow Service
provider_slug: fednow
scheme_count: 3
schemes:
- description: Each FedNow / FRFS API call presents a client PKI certificate. A separate certificate is required per environment (Test and Production); the same certificate may be reused across multiple APIs or a unique certificate may be requested per API. Certificates are provisioned through the credential-gated FedLine Developer platform.
  name: ClientCertificate
  type: mutualTLS
- description: A Client ID accompanies the certificate to identify the calling institution and its API entitlements.
  in: header
  name: ClientID
  type: apiKey
- description: FedLine multi-factor authentication security tokens gate access to the FedLine Developer platform where API credentials (Client ID + certificate) are managed. This layers institution-level MFA on top of the per-request certificate auth.
  name: FedLineSecurityToken
  type: mfa
slug: fednow-authentication
source_filename: fednow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://www.frbservices.org/fedline-solutions/fedline-developer/fednow-apis\ndocs: https://www.frbservices.org/fedline-solutions/fedline-developer\nsummary:\n  types: [mutualTLS, apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  gated: true\n  audience: enrolled financial institutions (FedNow / FedLine participants)\nschemes:\n- name: ClientCertificate\n  type: mutualTLS\n  description: >-\n    Each FedNow / FRFS API call presents a client PKI certificate. A separate\n    certificate is required per environment (Test and Production); the same\n    certificate may be reused across multiple APIs or a unique certificate may be\n    requested per API. Certificates are provisioned through the credential-gated\n    FedLine Developer platform.\n- name: ClientID\n  type: apiKey\n  in: header\n  description: >-\n    A Client ID accompanies the certificate to identify the calling institution\n    and its API entitlements.\n- name:\
  \ FedLineSecurityToken\n  type: mfa\n  description: >-\n    FedLine multi-factor authentication security tokens gate access to the FedLine\n    Developer platform where API credentials (Client ID + certificate) are managed.\n    This layers institution-level MFA on top of the per-request certificate auth.\nnotes: >-\n  FedNow is not a self-serve public API. Authentication is layered: FedLine MFA\n  security tokens to reach the developer platform, then Client ID + a\n  per-environment PKI client certificate on each API request. No OAuth2/OpenID\n  Connect flow and no public API key self-service are published; onboarding is\n  restricted to enrolled U.S. financial institutions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fednow/refs/heads/main/authentication/fednow-authentication.yml
summary_line: mutualTLS/apiKey · 3 schemes
tags:
- Payments
- United States
- Real-Time Payments
- Instant Payments
- ISO 20022
- Account-to-Account
- Scheme Operator
- Federal Reserve
---
