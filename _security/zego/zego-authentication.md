---
api_key_in:
- header
api_specs:
- filename: zego-partner-openapi.yml
  format: yaml
  label: Zego Partner API
  slug: zego-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zego/refs/heads/main/openapi/zego-partner-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Zego Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zego secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zego
provider_slug: zego
scheme_count: 1
schemes:
- description: Partner authorization token issued by the Zego Partnerships Manager.
  in: header
  name: partnerToken
  parameter: Authorization
  sources:
  - openapi/zego-partner-openapi.yml
  type: apiKey
slug: zego-authentication
source_filename: zego-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.zego.com/\ndocs: https://developer.zego.com/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nnotes: >-\n  The Zego Partner API uses token-based authentication. Partners are issued an\n  authorization token by the Zego Partnerships Manager and send it in the\n  Authorization header on every request. There is no self-serve OAuth flow; the\n  API is partner/work-provider gated. Inbound webhooks are authenticated by\n  Zego with an X-ZEGO-SIGNATURE header on the request.\nschemes:\n  - name: partnerToken\n    type: apiKey\n    in: header\n    parameter: Authorization\n    sources: [openapi/zego-partner-openapi.yml]\n    description: >-\n      Partner authorization token issued by the Zego Partnerships Manager.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zego/refs/heads/main/authentication/zego-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Insurance
- Insurtech
- Motor Insurance
- Gig Economy
- Telematics
- Fleet Insurance
- Public Liability
- Partner API
---
