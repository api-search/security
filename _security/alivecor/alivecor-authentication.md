---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Alivecor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alivecor secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Alivecor
provider_slug: alivecor
scheme_count: 1
schemes:
- description: The AliveCor API (cloud access to patient ECG data via KardiaPro) uses standard REST over HTTPS with API-key authentication, described by AliveCor as supporting HIPAA-compliant access to patient data.
  in: header
  name: apiKey
  sources:
  - https://alivecor.com/data-integration
  type: apiKey
slug: alivecor-authentication
source_filename: alivecor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://alivecor.com/data-integration\ndocs: https://alivecor.com/data-integration\nnote: >-\n  Derived from the published data-integration description; AliveCor does not\n  expose a public OpenAPI or developer portal (API access is gated behind a\n  commercial agreement), so this profile reflects the documented auth model\n  rather than a machine-readable spec.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  description: >-\n    The AliveCor API (cloud access to patient ECG data via KardiaPro) uses\n    standard REST over HTTPS with API-key authentication, described by AliveCor\n    as supporting HIPAA-compliant access to patient data.\n  sources: [https://alivecor.com/data-integration]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alivecor/refs/heads/main/authentication/alivecor-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Digital Health
- ECG
- Cardiology
- Medical Devices
- Remote Patient Monitoring
- Artificial Intelligence
- Health Data
---
