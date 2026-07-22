---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Liveaction Authentication
name_suffix: Authentication
oauth_flows: []
overview: LiveAction secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LiveAction
provider_slug: liveaction
scheme_count: 2
schemes:
- description: API token used to authenticate against the LiveWire / Omnipeek Capture Engine REST-API. Tokens are created and revoked from Omnipeek (Managing API Tokens) and passed on each REST-API request.
  in: header
  name: LiveWireCaptureEngineApiToken
  product: LiveWire / Omnipeek
  sources:
  - https://docs.liveaction.com/LiveWire/LiveWire%20User%20Guide/LiveWire_API_Tokens.5.1
  type: apiKey
- description: Token-based authentication for the LiveNX REST API used for automation and integration against a customer-operated LiveNX deployment.
  in: header
  name: LiveNXRestApiToken
  product: LiveNX
  sources:
  - https://docs.liveaction.com/
  type: apiKey
slug: liveaction-authentication
source_filename: liveaction-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.liveaction.com/LiveWire/LiveWire%20User%20Guide/LiveWire_API_Tokens.5.1\ndocs: https://docs.liveaction.com/\nnotes: >-\n  LiveAction exposes a product-embedded REST API surface rather than a public,\n  hosted developer API. The LiveWire / Omnipeek \"Capture Engine REST-API\" is\n  authenticated with API tokens that are created and managed inside Omnipeek;\n  once issued, the token is presented on REST-API calls. LiveNX likewise exposes\n  a REST API for automation against a customer-operated appliance. No public\n  OpenAPI/Swagger specification is published (API reference is served from the\n  in-product admin/user menu), so this profile is captured from the docs rather\n  than derived from a spec. There is no fixed public base URL — each API runs on\n  the customer's own LiveWire/LiveNX/Omnipeek deployment.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: LiveWireCaptureEngineApiToken\n\
  \  type: apiKey\n  in: header\n  description: >-\n    API token used to authenticate against the LiveWire / Omnipeek Capture\n    Engine REST-API. Tokens are created and revoked from Omnipeek (Managing API\n    Tokens) and passed on each REST-API request.\n  product: LiveWire / Omnipeek\n  sources:\n  - https://docs.liveaction.com/LiveWire/LiveWire%20User%20Guide/LiveWire_API_Tokens.5.1\n- name: LiveNXRestApiToken\n  type: apiKey\n  in: header\n  description: >-\n    Token-based authentication for the LiveNX REST API used for automation and\n    integration against a customer-operated LiveNX deployment.\n  product: LiveNX\n  sources:\n  - https://docs.liveaction.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liveaction/refs/heads/main/authentication/liveaction-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Network Monitoring
- Network Observability
- Network Performance Monitoring
- Packet Capture
- Network Forensics
- SD-WAN
- Telemetry
---
