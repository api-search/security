---
api_key_in: []
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Blassa Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blassa Inc. secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blassa Inc.
provider_slug: blassa-inc
scheme_count: 1
schemes:
- description: API key issued per account/plan from the Blassa business dashboard (https://business.blassa.io). Presented on each API request. Transport (header vs. query) per the Blassa API reference.
  name: apiKey
  official: true
  sources:
  - https://blassa.io/pricing
  - https://blassa.readme.io/
  type: apiKey
slug: blassa-inc-authentication
source_filename: blassa-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://blassa.io/pricing\ndocs: https://blassa.readme.io/\nsummary:\n  types:\n  - apiKey\n  notes: >-\n    Blassa is authenticated with API keys. Every plan includes API access with a\n    key; the Enterprise plan explicitly grants \"multiple API keys\". The exact key\n    transport (header name / query parameter) is documented in the Blassa ReadMe\n    developer portal but was not captured verbatim here (the portal is bot/rate\n    protected). No OpenAPI securitySchemes were available to derive from.\nschemes:\n- name: apiKey\n  type: apiKey\n  description: >-\n    API key issued per account/plan from the Blassa business dashboard\n    (https://business.blassa.io). Presented on each API request. Transport\n    (header vs. query) per the Blassa API reference.\n  official: true\n  sources:\n  - https://blassa.io/pricing\n  - https://blassa.readme.io/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blassa-inc/refs/heads/main/authentication/blassa-inc-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Location Intelligence
- Geocoding
- Address Verification
- Maps
- Logistics
- Last-Mile Delivery
- E-commerce
- Middle East
- Africa
---
