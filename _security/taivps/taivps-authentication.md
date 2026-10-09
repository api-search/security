---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Taivps Authentication
name_suffix: Authentication
oauth_flows: []
overview: TaiVPS declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: TaiVPS
provider_slug: taivps
scheme_count: 1
schemes:
- description: Every documented endpoint is a POST to https://taivps.net/api/<name>.php taking a required body parameter "token" (String, "Token API").
  in: body
  name: token
  parameter: token
  type: apiKey
slug: taivps-authentication
source_filename: taivps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: https://taivps.net/api-docs\ndocs: https://taivps.net/api-docs\nschemes:\n- name: token\n  type: apiKey\n  in: body\n  parameter: token\n  description: 'Every documented endpoint is a POST to https://taivps.net/api/<name>.php taking a required body parameter \"token\" (String, \"Token API\").'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taivps/refs/heads/main/authentication/taivps-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Cloud VPS
- Web Hosting
- Reseller Hosting
- Domains
- Infrastructure
- Vietnam
---
