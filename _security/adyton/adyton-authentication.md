---
api_key_in: []
auth_types:
- smartcard
- webauthn
- oauth2
- mutualTLS
- sso
description: ''
kind: authentication
layout: security
method: searched
name: Adyton Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adyton secures its APIs with smartcard, webauthn, oauth2, mutualTLS, and sso across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Adyton
provider_slug: adyton
scheme_count: 6
schemes:
- description: Common Access Card (CAC) authentication
  name: cac
  type: smartcard
- description: Personal Identity Verification (PIV) card authentication
  name: piv
  type: smartcard
- description: WebAuthn / FIDO2 phishing-resistant authenticators
  name: webauthn
  type: webauthn
- description: OAuth2 supported for integrations to legacy defense infrastructure and cloud APIs
  name: oauth2
  type: oauth2
- description: Client-certificate (mutual TLS) authentication for integrations
  name: client-certificate
  type: mutualTLS
- description: Flexible enterprise SSO integration
  name: sso
  type: sso
slug: adyton-authentication
source_filename: adyton-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://www.adyton.com/resources/security\nnote: >-\n  Authentication mechanisms as documented on Adyton's Security resource page for the\n  Adyton Operations Kit (AOK) / Atlas platform. Adyton publishes no public developer\n  API or OpenAPI, so this profile is derived from documented product auth support\n  rather than a machine-readable securitySchemes block.\nsummary:\n  types: [smartcard, webauthn, oauth2, mutualTLS, sso]\n  mfa: true\n  device_authentication: true\nschemes:\n- name: cac\n  type: smartcard\n  description: 'Common Access Card (CAC) authentication'\n- name: piv\n  type: smartcard\n  description: 'Personal Identity Verification (PIV) card authentication'\n- name: webauthn\n  type: webauthn\n  description: 'WebAuthn / FIDO2 phishing-resistant authenticators'\n- name: oauth2\n  type: oauth2\n  description: 'OAuth2 supported for integrations to legacy defense infrastructure and cloud APIs'\n- name: client-certificate\n\
  \  type: mutualTLS\n  description: 'Client-certificate (mutual TLS) authentication for integrations'\n- name: sso\n  type: sso\n  description: 'Flexible enterprise SSO integration'\ncontrols:\n  rbac: true\n  multi_factor: true\n  device_authentication: true\n  remote_wipe: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adyton/refs/heads/main/authentication/adyton-authentication.yml
summary_line: smartcard/webauthn/oauth2/mutualTLS/sso · 6 schemes
tags:
- Company
- Enterprise Saas
- Defense
- Zero Trust
- Mobile
- Security
- Personnel Accountability
- Logistics
- GovTech
---
