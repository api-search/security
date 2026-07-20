---
api_key_in: []
auth_types:
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Alkami Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alkami secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Alkami
provider_slug: alkami
scheme_count: 1
schemes:
- description: OpenID Connect based authentication for Alkami's D2C, B2B, and Open Banking REST APIs. Discovery/issuer details are provided to authorized financial institutions and fintech partners in the DevPortal.
  name: openIdConnect
  sources:
  - https://www.alkami.com/build-with-us/developers/
  type: openIdConnect
slug: alkami-authentication
source_filename: alkami-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://www.alkami.com/build-with-us/developers/\ndocs: https://developer.alkami.com\nsummary:\n  types: [openIdConnect]\n  oauth2_flows: []\n  note: >-\n    Alkami documents that its digital-banking APIs are \"built on OpenID Connect,\n    providing secure authentication without exposing PII.\" Full authentication\n    details (endpoints, flows, scopes, client registration) are published inside\n    the gated Alkami DevPortal at developer.alkami.com and are not available on\n    the public marketing surface.\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  description: >-\n    OpenID Connect based authentication for Alkami's D2C, B2B, and Open Banking\n    REST APIs. Discovery/issuer details are provided to authorized financial\n    institutions and fintech partners in the DevPortal.\n  sources:\n  - https://www.alkami.com/build-with-us/developers/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alkami/refs/heads/main/authentication/alkami-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Company
- Fintech
- Digital Banking
- Banking
- Credit Unions
- Financial Services
- Open Banking
- APIs
- SDK
---
