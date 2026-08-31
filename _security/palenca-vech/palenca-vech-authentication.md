---
api_key_in: []
api_specs:
- filename: palenca-vech-admin-api-openapi.yml
  format: yaml
  label: Palenca (Vech) admin API
  slug: palenca-vech-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/openapi/palenca-vech-admin-api-openapi.yml
- filename: palenca-vech-check-platform-health-api-openapi.yml
  format: yaml
  label: Palenca (Vech) Check Platform Health API
  slug: palenca-vech-check-platform-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/openapi/palenca-vech-check-platform-health-api-openapi.yml
- filename: palenca-vech-console-api-openapi.yml
  format: yaml
  label: Palenca (Vech) console API
  slug: palenca-vech-console-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/openapi/palenca-vech-console-api-openapi.yml
- filename: palenca-vech-ping-api-openapi.yml
  format: yaml
  label: Palenca (Vech) Ping API
  slug: palenca-vech-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/openapi/palenca-vech-ping-api-openapi.yml
- filename: palenca-vech-pong-api-openapi.yml
  format: yaml
  label: Palenca (Vech) Pong API
  slug: palenca-vech-pong-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/openapi/palenca-vech-pong-api-openapi.yml
- filename: palenca-vech-v1-api-openapi.yml
  format: yaml
  label: Palenca (Vech) v1 API
  slug: palenca-vech-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/openapi/palenca-vech-v1-api-openapi.yml
- filename: palenca-vech-version-api-openapi.yml
  format: yaml
  label: Palenca (Vech) Version API
  slug: palenca-vech-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/openapi/palenca-vech-version-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Palenca Vech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Palenca (Vech) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Palenca (Vech)
provider_slug: palenca-vech
scheme_count: 1
schemes:
- description: Private API key issued per environment. Retrieve from the Console at https://console.palenca.com/developers/api. Sent on almost all routes.
  environments:
  - base_url: https://sandbox.palenca.com
    name: sandbox
  - base_url: https://api.palenca.com
    name: production
  id: api_key
  in: header
  name: x-api-key
  type: apiKey
slug: palenca-vech-authentication
source_filename: palenca-vech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developers.palenca.com/docs/environments-and-authentication\napi: Palenca API\nsummary: >-\n  Palenca authenticates every request with a private API key sent in the x-api-key\n  request header. Separate keys exist for the sandbox and production environments.\n  The OpenAPI does not declare securitySchemes; this profile is sourced from the\n  published auth documentation.\ntransport:\n  tls_min_version: '1.3'\n  https_only: true\n  certificate_pinning: discouraged\n  required_headers:\n  - name: Content-Type\n    value: application/json\nschemes:\n- id: api_key\n  type: apiKey\n  in: header\n  name: x-api-key\n  description: >-\n    Private API key issued per environment. Retrieve from the Console at\n    https://console.palenca.com/developers/api. Sent on almost all routes.\n  environments:\n  - name: sandbox\n    base_url: https://sandbox.palenca.com\n  - name: production\n    base_url: https://api.palenca.com\noauth2:\
  \ false\nopenid_connect: false\nmutual_tls: false\nkey_management:\n  console_url: https://console.palenca.com/developers/api\n  environments: [sandbox, production]\ndocs: https://developers.palenca.com/docs/environments-and-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palenca-vech/refs/heads/main/authentication/palenca-vech-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Income Verification
- Employment Verification
- Fintech
- Gig Economy
- Latin America
- Identity
---
