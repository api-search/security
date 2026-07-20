---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cloudgenix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudgenix secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cloudgenix
provider_slug: cloudgenix
scheme_count: 1
schemes:
- description: CloudGenix Cloud Controller auth token, presented on every API request.
  in: header
  name: authToken
  parameter: X-Auth-Token
  sources:
  - https://github.com/CloudGenix/sdk-python
  type: apiKey
slug: cloudgenix-authentication
source_filename: cloudgenix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/CloudGenix/sdk-python\ndocs: https://developers.cloudgenix.com/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  notes: >-\n    Token-based authentication. Callers obtain an auth token (via interactive\n    login, SAML 2.0 SSO, or a static AUTH_TOKEN) and present it on every request\n    in the X-Auth-Token header against the CloudGenix Cloud Controller. MSP /\n    ESP tenant switching is supported by the SDK.\nschemes:\n  - name: authToken\n    type: apiKey\n    in: header\n    parameter: X-Auth-Token\n    description: CloudGenix Cloud Controller auth token, presented on every API request.\n    sources: [https://github.com/CloudGenix/sdk-python]\nlogin_methods:\n  - interactive\n  - saml2.0\n  - static-auth-token\ncontroller_default: https://api.elcapitan.cloudgenix.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudgenix/refs/heads/main/authentication/cloudgenix-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- SD-WAN
- Networking
- Cloud
- Software Defined Networking
- Network Automation
- SASE
- Infrastructure
---
