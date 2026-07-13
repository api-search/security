---
api_key_in:
- query
api_specs:
- filename: trello-rest-api-openapi.yml
  format: yaml
  label: Trello REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-rest-api-openapi.yml
- filename: trello-webhooks-asyncapi.yml
  format: yaml
  label: Trello Webhooks API
  slug: webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/asyncapi/trello-webhooks-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trello Authentication
name_suffix: Authentication
oauth_flows: []
overview: trello secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: trello
provider_slug: trello
scheme_count: 2
schemes:
- description: Your Trello API key, obtained from the Power-Ups admin page at https://trello.com/power-ups/admin.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/trello-rest-api-openapi.yml
  type: apiKey
- description: A user token that grants access to Trello resources. Obtained by authorizing via the /1/authorize route or OAuth 1.0.
  in: query
  name: apiToken
  parameter: token
  sources:
  - openapi/trello-rest-api-openapi.yml
  type: apiKey
slug: trello-authentication
source_filename: trello-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trello-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: Your Trello API key, obtained from the Power-Ups admin page at https://trello.com/power-ups/admin.\n  sources:\n  - openapi/trello-rest-api-openapi.yml\n- name: apiToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: A user token that grants access to Trello resources. Obtained by authorizing\n    via the /1/authorize route or OAuth 1.0.\n  sources:\n  - openapi/trello-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/authentication/trello-authentication.yml
summary_line: apiKey · 2 schemes
tags: []
---
