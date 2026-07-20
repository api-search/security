---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Intellectible Authentication
name_suffix: Authentication
oauth_flows: []
overview: Intellectible secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Intellectible
provider_slug: intellectible
scheme_count: 1
schemes:
- in: header
  key_management: https://app.intellectible.com
  name: apiKeyAuth
  parameter_name: Authorization
  scheme_note: 'The API key value is sent directly in the Authorization request header (e.g. "Authorization: API_KEY") - it is not prefixed with "Bearer". API keys are created in the app under the Accounts section and are scoped to project data, so they must be kept secret.'
  sources:
  - https://docs.intellectible.com/docs/api-reference/intro
  type: apiKey
slug: intellectible-authentication
source_filename: intellectible-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.intellectible.com/docs/api-reference/intro\ndocs: https://docs.intellectible.com/docs/api-reference/intro\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  scheme_note: >-\n    The API key value is sent directly in the Authorization request header\n    (e.g. \"Authorization: API_KEY\") - it is not prefixed with \"Bearer\". API keys\n    are created in the app under the Accounts section and are scoped to project\n    data, so they must be kept secret.\n  key_management: https://app.intellectible.com\n  sources:\n  - https://docs.intellectible.com/docs/api-reference/intro\nnotes: >-\n  No OpenAPI/Swagger specification is published for the Intellectible Public API,\n  so this profile was captured from the provider's API reference documentation\n  rather than derived from a spec. Only a single\
  \ API-key scheme is documented;\n  no OAuth2, OpenID Connect, or scope surface is present, so scopes/ is not\n  applicable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intellectible/refs/heads/main/authentication/intellectible-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Government
- GovCon
- Proposals
- CRM
- Workflow Automation
- Pricing
- Knowledge Management
- Enterprise Software
- Professional Services
---
