---
api_key_in:
- body
api_specs:
- filename: arkose-labs-verify-openapi.yml
  format: yaml
  label: Arkose Labs Verify API
  slug: arkose-labs-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkose-labs/refs/heads/main/openapi/arkose-labs-verify-openapi.yml
- filename: arkose-labs-edge-openapi.yml
  format: yaml
  label: Arkose Labs Edge API
  slug: arkose-labs-edge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arkose-labs/refs/heads/main/openapi/arkose-labs-edge-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Arkose Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arkose Labs secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Arkose Labs
provider_slug: arkose-labs
scheme_count: 2
schemes:
- description: Server-side secret paired with the client-side public key. Sent in the application/json POST body to the Verify API. Never expose client-side.
  in: body
  name: privateKey
  parameter: private_key
  sources:
  - openapi/arkose-labs-verify-openapi.yml
  type: apiKey
  used_by: Arkose Labs Verify API
- description: Account public key used as a path segment on the Edge API endpoint (/api/edge/v1/{public_key}) and to load the client-side script.
  in: path
  name: publicKey
  parameter: public_key
  sources:
  - openapi/arkose-labs-edge-openapi.yml
  type: apiKey
  used_by: Arkose Labs Edge API
slug: arkose-labs-authentication
source_filename: arkose-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.arkoselabs.com/docs/calling-verify-v4-api\ndocs: https://developer.arkoselabs.com/docs/arkose-labs-api-guide\nsummary:\n  types: [apiKey]\n  api_key_in: [body]\n  oauth2_flows: []\n  notes: >-\n    Arkose Labs uses a public/private key pair per customer account. The public\n    key is embedded client-side to load the enforcement/detection script; the\n    private key is a server-side secret passed in the JSON body of the Verify\n    API request. There is no OAuth or bearer-token scheme. The Edge API is keyed\n    by the public key in the request path.\nschemes:\n  - name: privateKey\n    type: apiKey\n    in: body\n    parameter: private_key\n    used_by: Arkose Labs Verify API\n    description: >-\n      Server-side secret paired with the client-side public key. Sent in the\n      application/json POST body to the Verify API. Never expose client-side.\n    sources: [openapi/arkose-labs-verify-openapi.yml]\n\
  \  - name: publicKey\n    type: apiKey\n    in: path\n    parameter: public_key\n    used_by: Arkose Labs Edge API\n    description: >-\n      Account public key used as a path segment on the Edge API endpoint\n      (/api/edge/v1/{public_key}) and to load the client-side script.\n    sources: [openapi/arkose-labs-edge-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arkose-labs/refs/heads/main/authentication/arkose-labs-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Enterprise
- Security
- Bot Management
- Fraud Prevention
- Authentication
- Account Security
- Bot Detection
- Risk Scoring
- CAPTCHA
---
