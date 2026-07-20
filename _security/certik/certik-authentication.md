---
api_key_in:
- header
api_specs:
- filename: certik-skynet-openapi.yml
  format: yaml
  label: CertiK Partner (Skynet) API
  slug: certik-partner-skynet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certik/refs/heads/main/openapi/certik-skynet-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Certik Authentication
name_suffix: Authentication
oauth_flows: []
overview: CertiK secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CertiK
provider_slug: certik
scheme_count: 1
schemes:
- description: Partner API key issued by the CertiK Business Team, sent on every request in the X-Certik-Api-Key header.
  in: header
  name: CertikApiKey
  parameter: X-Certik-Api-Key
  sources:
  - openapi/certik-skynet-openapi.yml
  type: apiKey
slug: certik-authentication
source_filename: certik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/certik-skynet-openapi.yml\ndocs: https://api.certik-skynet.com/public-docs/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: CertikApiKey\n  type: apiKey\n  in: header\n  parameter: X-Certik-Api-Key\n  description: Partner API key issued by the CertiK Business Team, sent on every request in\n    the X-Certik-Api-Key header.\n  sources:\n  - openapi/certik-skynet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certik/refs/heads/main/authentication/certik-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cybersecurity
- Web3
- Blockchain
- Smart Contract Security
- Security Auditing
- Threat Intelligence
---
