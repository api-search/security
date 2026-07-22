---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Ozforex Authentication
name_suffix: Authentication
oauth_flows: []
overview: OFX (OzForex) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OFX (OzForex)
provider_slug: ozforex
scheme_count: 1
schemes:
- description: API key issued to approved partners for authenticating requests to the OFX Payments API. Obtained via partner onboarding at developer.ofx.com and the business registration flow (app.ofx.com/registration).
  in: header
  name: apiKey
  sources:
  - https://www.ofx.com/en-us/partner-with-us/api/
  type: apiKey
slug: ozforex-authentication
source_filename: ozforex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.ofx.com/en-us/partner-with-us/api/\ndocs: https://developer.ofx.com/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  notes: >-\n    OFX documents its partner Payments API as a RESTful API secured with API keys.\n    A full securityScheme profile could not be derived because OFX publishes no\n    public OpenAPI specification — the developer portal (developer.ofx.com) gates\n    the API reference behind partner onboarding. Values below are from the public\n    API partner page, not a machine-readable spec.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  description: >-\n    API key issued to approved partners for authenticating requests to the OFX\n    Payments API. Obtained via partner onboarding at developer.ofx.com and the\n    business registration flow (app.ofx.com/registration).\n  sources: [https://www.ofx.com/en-us/partner-with-us/api/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ozforex/refs/heads/main/authentication/ozforex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer
- Money Transfer
- Foreign Exchange
- International Payments
- Payments
- Currency
- Fintech
---
