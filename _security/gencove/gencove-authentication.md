---
api_key_in:
- header
api_specs:
- filename: gencove-openapi-original.json
  format: json
  label: Gencove Back API
  slug: gencove-back-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/openapi/gencove-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Gencove Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gencove secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gencove
provider_slug: gencove
scheme_count: 2
schemes:
- description: 'Authorization header content formatted as: `Api-Key <API-key>`

    Obtain an API key through Gencove''s web UI (Account Settings -> API Keys)

    or the user-api-key endpoint.'
  docs: https://docs.gencove.com/base/getting-started/
  in: header
  name: API key
  parameter: Authorization
  scheme_hint: Api-Key <API-key>
  sources:
  - openapi/gencove-openapi-original.json
  type: apiKey
- description: 'Authorization header content formatted as: `Bearer <json-web-token>`

    Obtain an access token using the jwt-create endpoint; refresh via

    jwt-refresh and verify via jwt-verify.'
  in: header
  name: JWT
  parameter: Authorization
  scheme_hint: Bearer <json-web-token>
  sources:
  - openapi/gencove-openapi-original.json
  type: apiKey
slug: gencove-authentication
source_filename: gencove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/gencove-openapi-original.json\ndocs: https://docs.gencove.com/base/getting-started/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    Gencove uses a static API key by default (Authorization: Api-Key <key>),\n    issued from the dashboard under Account Settings -> API Keys. A short-lived\n    JWT bearer token flow is also available via the jwt-create endpoint\n    (Authorization: Bearer <jwt>). Email/password env vars ($GENCOVE_EMAIL /\n    $GENCOVE_PASSWORD) can be used by the CLI to obtain a token but cannot be\n    combined with $GENCOVE_API_KEY.\nschemes:\n- name: API key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_hint: 'Api-Key <API-key>'\n  description: |-\n    Authorization header content formatted as: `Api-Key <API-key>`\n    Obtain an API key through Gencove's web UI (Account Settings -> API Keys)\n    or the user-api-key endpoint.\n  docs: https://docs.gencove.com/base/getting-started/\n\
  \  sources:\n  - openapi/gencove-openapi-original.json\n- name: JWT\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_hint: 'Bearer <json-web-token>'\n  description: |-\n    Authorization header content formatted as: `Bearer <json-web-token>`\n    Obtain an access token using the jwt-create endpoint; refresh via\n    jwt-refresh and verify via jwt-verify.\n  sources:\n  - openapi/gencove-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gencove/refs/heads/main/authentication/gencove-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Health
- Genomics
- Sequencing
- Bioinformatics
- DNA
- Life Sciences
- Analytics
---
