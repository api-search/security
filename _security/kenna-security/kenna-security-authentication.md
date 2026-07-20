---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Kenna Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kenna Security secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kenna Security
provider_slug: kenna-security
scheme_count: 1
schemes:
- description: All requests must include an X-Risk-Token header whose value is the API token generated in the Cisco Vulnerability Management UI under Settings > API Keys. API keys can be copied one time immediately after generation. All calls must be over HTTPS; plain HTTP requests fail.
  in: header
  name: XRiskToken
  parameter_name: X-Risk-Token
  sources:
  - https://apidocs.kennasecurity.com/reference/api-authentication
  type: apiKey
slug: kenna-security-authentication
source_filename: kenna-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://apidocs.kennasecurity.com/reference/api-authentication\ndocs: https://apidocs.kennasecurity.com/reference/api-authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: XRiskToken\n  type: apiKey\n  in: header\n  parameter_name: X-Risk-Token\n  description: >-\n    All requests must include an X-Risk-Token header whose value is the API token\n    generated in the Cisco Vulnerability Management UI under Settings > API Keys.\n    API keys can be copied one time immediately after generation. All calls must be\n    over HTTPS; plain HTTP requests fail.\n  sources:\n  - https://apidocs.kennasecurity.com/reference/api-authentication\nnotes:\n- The API base host matches the subscription subdomain; the documented example host is\n  api.kennasecurity.com. Verify the exact host on the Settings > API Keys page.\n- No OAuth2 / OpenID Connect flows are documented; authentication\
  \ is a single static\n  API-key token header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kenna-security/refs/heads/main/authentication/kenna-security-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cybersecurity
- Vulnerability Management
- Risk-Based Prioritization
- Threat Intelligence
- Security
- Cisco
- REST API
---
