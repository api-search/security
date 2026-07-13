---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Brave Browser Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brave secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brave
provider_slug: brave-browser
scheme_count: 1
schemes:
- in: header
  name: SubscriptionToken
  parameter: X-Subscription-Token
  sources:
  - openapi/brave-browser-openapi.yml
  type: apiKey
slug: brave-browser-authentication
source_filename: brave-browser-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/brave-browser-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SubscriptionToken\n  type: apiKey\n  in: header\n  parameter: X-Subscription-Token\n  sources:\n  - openapi/brave-browser-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/authentication/brave-browser-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Browser
- Search
- Privacy
- Chromium
- Web3
- AI
- Advertising
---
