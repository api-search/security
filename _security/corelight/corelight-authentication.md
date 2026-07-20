---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Corelight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Corelight secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Corelight
provider_slug: corelight
scheme_count: 2
schemes:
- description: 'HTTP Basic authentication against the Corelight Sensor. Two device API users exist: admin (unlimited access) and monitor (read-only access). API access must first be enabled through the device configuration interface and passwords set for both users.'
  name: basicAuth
  scheme: basic
  sources:
  - https://github.com/corelight/corelight-client
  type: http
- description: Authentication against a Corelight Fleet Manager additionally accepts a 2FA verification code (--mfa). Credentials are cached in ~/.corelight-client/credentials after first use.
  mfa: totp
  name: fleetMfa
  scheme: basic
  sources:
  - https://github.com/corelight/corelight-client
  type: http
slug: corelight-authentication
source_filename: corelight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/corelight/corelight-client\ndocs: https://github.com/corelight/corelight-client#access-and-authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  mfa: true\n  notes: >-\n    No public OpenAPI is published for the Corelight Sensor API (device-local,\n    account-gated). This profile is searched from the official corelight-client\n    documentation.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication against the Corelight Sensor. Two device API users\n    exist: admin (unlimited access) and monitor (read-only access). API access\n    must first be enabled through the device configuration interface and\n    passwords set for both users.\n  sources:\n  - https://github.com/corelight/corelight-client\n- name: fleetMfa\n  type: http\n  scheme: basic\n  mfa: totp\n  description: >-\n    Authentication against a Corelight Fleet Manager\
  \ additionally accepts a 2FA\n    verification code (--mfa). Credentials are cached in\n    ~/.corelight-client/credentials after first use.\n  sources:\n  - https://github.com/corelight/corelight-client\ntransport_security:\n  tls: required\n  custom_ca: supported\n  notes: >-\n    Client validates the device SSL certificate by default; a custom CA cert may\n    be supplied, and verification can be relaxed for lab devices.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corelight/refs/heads/main/authentication/corelight-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Cybersecurity
- Network Detection and Response
- NDR
- Network Security
- Threat Detection
- Zeek
- Incident Response
- Security
---
