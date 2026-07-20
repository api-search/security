---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Betterview Marketplace Authentication
name_suffix: Authentication
oauth_flows: []
overview: BetterView Marketplace secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BetterView Marketplace
provider_slug: betterview-marketplace
scheme_count: 1
schemes:
- description: Bearer token obtained via Betterview's documented authentication workflow; sent in the HTTP Authorization header on API requests.
  name: bearerAuth
  scheme: bearer
  sources:
  - https://betterview.readme.io/docs/authentication
  type: http
slug: betterview-marketplace-authentication
source_filename: betterview-marketplace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://betterview.readme.io/docs/authentication\ndocs: https://betterview.readme.io/docs/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Betterview's API is authenticated with a bearer token. Per the published\n    authentication guide, developers follow an authentication workflow to\n    retrieve a bearer token, which is then presented on subsequent API requests\n    to the Property Intelligence API. No OpenAPI/Swagger definition was\n    discoverable on the ReadMe-hosted developer portal, so this profile is\n    grounded in the documented auth workflow rather than a machine-readable\n    securityScheme.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token obtained via Betterview's documented authentication workflow;\n    sent in the HTTP Authorization header on API requests.\n  sources:\n  - https://betterview.readme.io/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betterview-marketplace/refs/heads/main/authentication/betterview-marketplace-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Property Intelligence
- Insurance
- Insurtech
- Geospatial
- Underwriting
- Property Data
- Risk
---
