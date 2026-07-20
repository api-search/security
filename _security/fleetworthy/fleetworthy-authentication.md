---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Fleetworthy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fleetworthy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fleetworthy
provider_slug: fleetworthy
scheme_count: 1
schemes:
- description: Azure API Management subscription key issued per product subscription from the developer portal. Header name is the Azure APIM default; confirm against the portal's per-API "Try it" console.
  in: header
  name: subscriptionKey
  parameter_name: Ocp-Apim-Subscription-Key
  source: https://developer.fleetworthy.com/
  type: apiKey
slug: fleetworthy-authentication
source_filename: fleetworthy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.fleetworthy.com/\ndocs: https://developer.fleetworthy.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    The Fleetworthy Compliance API is published through Azure API Management. Access requires signing\n    in with a CPSuite account on the developer portal, subscribing to a product, and requesting API\n    (subscription) keys. Requests to the gateway (api.fleetworthy.com) are authenticated with the\n    Azure API Management subscription key, passed by default in the Ocp-Apim-Subscription-Key request\n    header. Scope/permission model is governed by the product a subscription is granted against\n    (Read Reports, Asset Management, Driver Management).\nschemes:\n- name: subscriptionKey\n  type: apiKey\n  in: header\n  parameter_name: Ocp-Apim-Subscription-Key\n  description: >-\n    Azure API Management subscription key issued per product subscription from the developer portal.\n\
  \    Header name is the Azure APIM default; confirm against the portal's per-API \"Try it\" console.\n  source: https://developer.fleetworthy.com/\nonboarding:\n- Sign in with a CPSuite account at https://developer.fleetworthy.com/\n- Subscribe to a product and request API keys\n- Use the issued subscription key to call the gateway at https://api.fleetworthy.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fleetworthy/refs/heads/main/authentication/fleetworthy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fleet Management
- Compliance
- Transportation
- Trucking
- Safety
- Toll Management
- Weigh Station Bypass
- Logistics
---
