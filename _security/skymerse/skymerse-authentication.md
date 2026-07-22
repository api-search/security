---
api_key_in:
- header
api_specs:
- filename: skymerse-notamify-openapi-original.json
  format: json
  label: Notamify API V2
  slug: notamify-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skymerse/refs/heads/main/openapi/skymerse-notamify-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Skymerse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skymerse secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Skymerse
provider_slug: skymerse
scheme_count: 1
schemes:
- format: 'Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  in: header
  key_management: https://notamify.com/api-manager
  name: bearerAuth
  notes: Notamify API keys are passed as bearer tokens in the Authorization header. Generate and rotate keys in the API Manager. All endpoints are served exclusively over TLS; plain-HTTP requests are rejected. The Python SDK can read the token from the NOTAMIFY_TOKEN environment variable or ~/.config/notamify/config.json. No OAuth scopes are documented — access is a single API-key credential metered by a credit-based usage model.
  scheme: bearer
  sources:
  - openapi/skymerse-notamify-openapi-original.json
  type: http
slug: skymerse-authentication
source_filename: skymerse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/skymerse-notamify-openapi-original.json\ndocs: https://skymerse.gitbook.io/notamify-api/basics/authentication-guide\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer YOUR_API_KEY'\n  key_management: https://notamify.com/api-manager\n  notes: >-\n    Notamify API keys are passed as bearer tokens in the Authorization header.\n    Generate and rotate keys in the API Manager. All endpoints are served\n    exclusively over TLS; plain-HTTP requests are rejected. The Python SDK can\n    read the token from the NOTAMIFY_TOKEN environment variable or\n    ~/.config/notamify/config.json. No OAuth scopes are documented — access is a\n    single API-key credential metered by a credit-based usage model.\n  sources:\n  - openapi/skymerse-notamify-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skymerse/refs/heads/main/authentication/skymerse-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Aviation
- NOTAM
- Flight Operations
- Aeronautical
- Weather
- AI
- Webhooks
---
