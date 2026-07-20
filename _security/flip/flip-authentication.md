---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Flip Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flip secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flip
provider_slug: flip
scheme_count: 1
schemes:
- description: Flip for Business uses HTTP Basic authentication. The account secret key is sent as the Basic-auth username with an empty password. The secret key is retrieved from the Flip for Business dashboard (Integration / Developer settings). Separate keys exist for the sandbox and production environments.
  name: SecretKeyBasicAuth
  scheme: basic
  sources:
  - https://docs.flip.id/
  type: http
slug: flip-authentication
source_filename: flip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.flip.id/\ndocs: https://docs.flip.id/\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\n  extras: [ip-whitelisting, callback-token-validation]\nschemes:\n- name: SecretKeyBasicAuth\n  type: http\n  scheme: basic\n  description: >-\n    Flip for Business uses HTTP Basic authentication. The account secret key is\n    sent as the Basic-auth username with an empty password. The secret key is\n    retrieved from the Flip for Business dashboard (Integration / Developer\n    settings). Separate keys exist for the sandbox and production environments.\n  sources: [https://docs.flip.id/]\ncontrols:\n- id: ip-whitelisting\n  description: >-\n    Requests can be restricted to a set of whitelisted server IP addresses\n    configured in the Flip for Business dashboard.\n- id: callback-token-validation\n  description: >-\n    Incoming callbacks/webhooks carry a validation token that must\
  \ be verified\n    against the account's configured validation token before the payload is\n    trusted.\n- id: content-type-validation\n  description: >-\n    As of the 2025-12-07 security enhancement, requests are validated for a\n    correct Content-Type and an inquiry_key where applicable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flip/refs/heads/main/authentication/flip-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Payments
- Payment Gateway
- Money Transfer
- Disbursement
- Remittance
- Fintech
- Indonesia
- International Transfer
- Banking
---
