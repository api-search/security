---
api_key_in:
- header
api_specs:
- filename: browser-use-openapi.yml
  format: yaml
  label: Browser Use
  slug: browser-use
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/openapi/browser-use-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Browser Use Authentication
name_suffix: Authentication
oauth_flows: []
overview: Browser Use secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Browser Use
provider_slug: browser-use
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Browser-Use-API-Key
  sources:
  - openapi/browser-use-openapi.yml
  type: apiKey
slug: browser-use-authentication
source_filename: browser-use-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/browser-use-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Browser-Use-API-Key\n  sources:\n  - openapi/browser-use-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/browser-use/refs/heads/main/authentication/browser-use-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Automation
- Browser Automation
---
