---
api_key_in: []
api_specs:
- filename: kernel-openapi.yml
  format: yaml
  label: Kernel API
  slug: kernel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel-so/refs/heads/main/openapi/kernel-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kernel So Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kernel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kernel
provider_slug: kernel-so
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kernel-openapi.yml
  type: http
slug: kernel-so-authentication
source_filename: kernel-so-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kernel-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/kernel-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kernel-so/refs/heads/main/authentication/kernel-so-authentication.yml
summary_line: http · 1 scheme
tags:
- Agents
- AI
- Artificial Intelligence
- Browser Automation
- Browsers
- Computer Use
- Headless Browsers
- MCP
- Playwright
- Web Agents
---
