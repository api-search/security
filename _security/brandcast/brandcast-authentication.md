---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Brandcast Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brandcast secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brandcast
provider_slug: brandcast
scheme_count: 1
schemes:
- description: Brandcast API requests are authenticated with an API key sent in the x-api-key HTTP header over HTTPS. Keys are issued by Brandcast and are tied to the developer's Brandcast account. No OAuth or OpenID Connect flow is documented for the public API.
  in: header
  name: apiKey
  parameter_name: x-api-key
  sources:
  - https://developer.brandcast.io/
  transport: https-only
  type: apiKey
slug: brandcast-authentication
source_filename: brandcast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.brandcast.io/\ndocs: https://developer.brandcast.io/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  transport: https-only\n  description: >-\n    Brandcast API requests are authenticated with an API key sent in the\n    x-api-key HTTP header over HTTPS. Keys are issued by Brandcast and are\n    tied to the developer's Brandcast account. No OAuth or OpenID Connect\n    flow is documented for the public API.\n  sources:\n  - https://developer.brandcast.io/\nnotes: >-\n  Derived by searching the Brandcast developer documentation\n  (developer.brandcast.io, mirrored at api.brandcast.io). The provider does\n  not publish an OpenAPI/Swagger specification, so this profile is captured\n  from the documented authentication guidance rather than derived from a spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandcast/refs/heads/main/authentication/brandcast-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Enterprise Software
- No-Code
- Website Builder
- Content Management
- Digital Experience
- Web Design
- Brand Management
---
