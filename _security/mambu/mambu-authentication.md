---
api_key_in:
- header
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mambu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mambu secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mambu
provider_slug: mambu
scheme_count: 2
schemes:
- description: HTTP Basic authentication using a Mambu user's UI login credentials in the Authorization header as "Basic {base64(username:password)}". The user must hold a role/permissions with API access. HTTPS is required.
  name: basicAuth
  scheme: basic
  sources:
  - https://docs.mambu.com/api/pages/api-v2/authentication/
  type: http
- description: API key token passed in the apikey header. Currently an Early Access capability requiring activation through a Mambu Customer Success Manager.
  in: header
  name: apiKeyAuth
  parameter_name: apikey
  sources:
  - https://docs.mambu.com/api/pages/api-v2/authentication/
  type: apiKey
slug: mambu-authentication
source_filename: mambu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.mambu.com/api/pages/api-v2/authentication/\ndocs: https://docs.mambu.com/api/pages/api-v2/authentication/\nsummary:\n  types: [http, apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Mambu API v2 has no OAuth2 surface. Requests authenticate over HTTPS with\n    either HTTP Basic auth (Mambu UI username:password, base64 encoded) or an\n    API key supplied in the apikey request header. API keys are an Early Access\n    feature enabled via a Mambu Customer Success Manager.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication using a Mambu user's UI login credentials in the\n      Authorization header as \"Basic {base64(username:password)}\". The user must\n      hold a role/permissions with API access. HTTPS is required.\n    sources: [https://docs.mambu.com/api/pages/api-v2/authentication/]\n  - name: apiKeyAuth\n    type: apiKey\n\
  \    in: header\n    parameter_name: apikey\n    description: >-\n      API key token passed in the apikey header. Currently an Early Access\n      capability requiring activation through a Mambu Customer Success Manager.\n    sources: [https://docs.mambu.com/api/pages/api-v2/authentication/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mambu/refs/heads/main/authentication/mambu-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Fintech
- Banking
- Core Banking
- Lending
- Deposits
- Payments
- SaaS
- Embedded Finance
- Banking as a Service
---
