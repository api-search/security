---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Felh Magyar Zleti Infrastrukt Ra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Felhő — Magyar üzleti infrastruktúra secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Felhő — Magyar üzleti infrastruktúra
provider_slug: felh-magyar-zleti-infrastrukt-ra
scheme_count: 1
schemes:
- description: 'Send the API key as an HTTP bearer token: `Authorization: Bearer flh_live_…`. Keys are issued from the /app dashboard and are bound to a paid plan; a key on a free workspace returns HTTP 402 payment_required rather than 401, and starts working again when the plan is activated (no re-issue needed). The key is a secret — the provider explicitly warns against calling the API directly from a browser and instructs consumers to proxy requests through their own backend.'
  in: header
  key_prefix: flh_live_
  name: apiKey
  parameter_name: Authorization
  scheme_prefix: 'Bearer '
  sources:
  - llms-api-hu.txt
  type: apiKey
slug: felh-magyar-zleti-infrastrukt-ra-authentication
source_filename: felh-magyar-zleti-infrastrukt-ra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: https://felho.hu/llms-api-hu.txt (Felho API reference, \"Alapok\") + live 401 probe of https://felho.hu/api/v1/companies\ndocs: https://felho.hu/dokumentacio\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    scheme_prefix: 'Bearer '\n    key_prefix: flh_live_\n    description: >-\n      Send the API key as an HTTP bearer token: `Authorization: Bearer flh_live_…`. Keys are\n      issued from the /app dashboard and are bound to a paid plan; a key on a free workspace\n      returns HTTP 402 payment_required rather than 401, and starts working again when the plan\n      is activated (no re-issue needed). The key is a secret — the provider explicitly warns\n      against calling the API directly from a browser and instructs consumers to proxy requests\n      through their own backend.\n    sources: [llms-api-hu.txt]\n\
  observed:\n  probe: https://felho.hu/api/v1/companies?q=teszt\n  http_status: 401\n  body: '{\"error\":\"unauthorized\",\"message\":\"Missing API key. Send it as: Authorization: Bearer flh_...\"}'\n  checked: '2026-09-18'\nnotes: >-\n  Static bearer API key only. No OAuth 2.0 / OpenID Connect, no mTLS. Confirmed against the\n  published reference and the live unauthenticated 401 response.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/felh-magyar-zleti-infrastrukt-ra/refs/heads/main/authentication/felh-magyar-zleti-infrastrukt-ra-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company Data
- Business Verification
- Domains
- WHOIS/RDAP
- Hungary
- Registry Data
- Financial Data
---
