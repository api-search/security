---
api_key_in:
- header
api_specs:
- filename: leeo-insurance-services-fleet-openapi.yml
  format: yaml
  label: LEEO Fleet Telematics API
  slug: leeo-insurance-services-fleet-telematics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leeo-insurance-services/refs/heads/main/openapi/leeo-insurance-services-fleet-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Leeo Insurance Services Authentication
name_suffix: Authentication
oauth_flows: []
overview: LEEO Insurance Services secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LEEO Insurance Services
provider_slug: leeo-insurance-services
scheme_count: 1
schemes:
- description: Fleet-scoped API key issued from the LEEO dashboard Settings page, sent in the Authorization header prefixed with the literal `APIKEY `.
  docs: https://docs.leeoinsurance.com/leeo-apis/
  expiry_documented: false
  in: header
  key_source: LEEO dashboard, Settings page
  name: apiKeyAuth
  parameter: Authorization
  rotation_documented: false
  scope: fleet
  sources:
  - openapi/leeo-insurance-services-fleet-openapi.yml
  type: apiKey
  value_format: APIKEY <fm_api_key>
slug: leeo-insurance-services-authentication
source_filename: leeo-insurance-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/leeo-insurance-services-fleet-openapi.yml\ndocs: https://docs.leeoinsurance.com/leeo-apis/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  model: >-\n    A single fleet-scoped API key. There is no OAuth, no OIDC, no scope surface, and no per-user\n    identity — the key identifies the fleet and grants read access to that fleet's telematics data.\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  value_format: \"APIKEY <fm_api_key>\"\n  description: >-\n    Fleet-scoped API key issued from the LEEO dashboard Settings page, sent in the Authorization\n    header prefixed with the literal `APIKEY `.\n  key_source: LEEO dashboard, Settings page\n  scope: fleet\n  rotation_documented: false\n  expiry_documented: false\n  sources:\n  - openapi/leeo-insurance-services-fleet-openapi.yml\n  docs: https://docs.leeoinsurance.com/leeo-apis/\nrequired_headers:\n\
  - name: Authorization\n  value: \"APIKEY <fm_api_key>\"\n- name: Content-Type\n  value: application/json\nnotes: >-\n  The SDK side of the LEEO platform authenticates separately — mobile SDKs are initialized with\n  their own SDK key and a caller-supplied driver id, documented in the per-platform integration\n  guides rather than in the API reference.\nscopes:\n  supported: false\n  reason: API key authentication with no scope or permission surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leeo-insurance-services/refs/heads/main/authentication/leeo-insurance-services-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Insurance
- Insurtech
- Commercial Auto Insurance
- Telematics
- Fleet Management
- Driving Behavior
- Risk Management
- Managing General Agent
- Mobile SDK
---
