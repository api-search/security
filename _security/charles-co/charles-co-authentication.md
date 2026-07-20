---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Charles Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Charles Co secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Charles Co
provider_slug: charles-co
scheme_count: 2
schemes:
- description: After a successful login the SDK stores a token that is sent on subsequent requests (rehydrated via credentials.token). Requests are made against a per-tenant "universe" base host configured at init.
  name: bearerToken
  obtained_via: username-password login
  scheme: bearer
  source: https://github.com/c-commerce/charles-browser-sdk#usage
  type: http
- description: charles.auth.loginUsername({ username, password }) authenticates a client account and returns the session token used as the bearer credential.
  name: usernamePasswordLogin
  source: https://github.com/c-commerce/charles-browser-sdk#usage
  type: login
slug: charles-co-authentication
source_filename: charles-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://c-commerce.github.io/charles-browser-sdk/\ndocs: https://github.com/c-commerce/charles-browser-sdk#usage\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  login_flows:\n  - username-password\n  notes: >-\n    Documented from the first-party browser SDK. No public OpenAPI is published,\n    so schemes are captured from the SDK usage docs rather than derived from a\n    spec.\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: >-\n    After a successful login the SDK stores a token that is sent on subsequent\n    requests (rehydrated via credentials.token). Requests are made against a\n    per-tenant \"universe\" base host configured at init.\n  obtained_via: username-password login\n  source: https://github.com/c-commerce/charles-browser-sdk#usage\n- name: usernamePasswordLogin\n  type: login\n  description: >-\n    charles.auth.loginUsername({ username, password }) authenticates\
  \ a client\n    account and returns the session token used as the bearer credential.\n  source: https://github.com/c-commerce/charles-browser-sdk#usage\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charles-co/refs/heads/main/authentication/charles-co-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Conversational Commerce
- Messaging
- WhatsApp
- CRM
- Customer Support
- E-Commerce
- AI Agents
---
