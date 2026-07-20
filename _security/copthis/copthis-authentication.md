---
api_key_in: []
api_specs:
- filename: copthis-partner-api-openapi.yml
  format: yaml
  label: Merchbar Partner API
  slug: merchbar-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/copthis/refs/heads/main/openapi/copthis-partner-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Copthis Authentication
name_suffix: Authentication
oauth_flows: []
overview: CopThis secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CopThis
provider_slug: copthis
scheme_count: 1
schemes:
- description: HTTP Basic Authentication over HTTPS. Merchbar recommends a randomly generated token as the username and a blank password. Non-TLS connections are rejected.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/copthis-partner-api-openapi.yml
  type: http
slug: copthis-authentication
source_filename: copthis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/copthis-partner-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication over HTTPS. Merchbar recommends a randomly generated\n    token as the username and a blank password. Non-TLS connections are rejected.\n  sources:\n  - openapi/copthis-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/copthis/refs/heads/main/authentication/copthis-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Music
- Merchandise
- E-Commerce
- Retail
- Orders
- Fulfillment
- Partner API
- Marketplace
---
