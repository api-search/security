---
api_key_in: []
api_specs:
- filename: kernel-openapi-original.yml
  format: yaml
  label: Kernel API
  slug: kernel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kernel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kernel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kernel
provider_slug: kernel
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kernel-openapi-original.yml
  type: http
slug: kernel-authentication
source_filename: kernel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/kernel-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/kernel-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/authentication/kernel-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Browser Automation
- Web Agents
- Browser Infrastructure
- AI Agents
- Playwright
- Cloud Browsers
- Computer Use
- MCP
- Managed Auth
---
