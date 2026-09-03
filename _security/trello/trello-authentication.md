---
api_key_in:
- query
api_specs:
- filename: trello-webhooks-asyncapi.yml
  format: yaml
  label: Trello Webhooks API
  slug: webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/asyncapi/trello-webhooks-asyncapi.yml
- filename: trello-actions-api-openapi.yml
  format: yaml
  label: trello Actions API
  slug: trello-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-actions-api-openapi.yml
- filename: trello-boards-api-openapi.yml
  format: yaml
  label: trello Boards API
  slug: trello-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-boards-api-openapi.yml
- filename: trello-cards-api-openapi.yml
  format: yaml
  label: trello Cards API
  slug: trello-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-cards-api-openapi.yml
- filename: trello-checklists-api-openapi.yml
  format: yaml
  label: trello Checklists API
  slug: trello-checklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-checklists-api-openapi.yml
- filename: trello-customfields-api-openapi.yml
  format: yaml
  label: trello CustomFields API
  slug: trello-customfields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-customfields-api-openapi.yml
- filename: trello-labels-api-openapi.yml
  format: yaml
  label: trello Labels API
  slug: trello-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-labels-api-openapi.yml
- filename: trello-lists-api-openapi.yml
  format: yaml
  label: trello Lists API
  slug: trello-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-lists-api-openapi.yml
- filename: trello-members-api-openapi.yml
  format: yaml
  label: trello Members API
  slug: trello-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-members-api-openapi.yml
- filename: trello-notifications-api-openapi.yml
  format: yaml
  label: trello Notifications API
  slug: trello-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-notifications-api-openapi.yml
- filename: trello-organizations-api-openapi.yml
  format: yaml
  label: trello Organizations API
  slug: trello-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-organizations-api-openapi.yml
- filename: trello-plugins-api-openapi.yml
  format: yaml
  label: trello Plugins API
  slug: trello-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-plugins-api-openapi.yml
- filename: trello-search-api-openapi.yml
  format: yaml
  label: trello Search API
  slug: trello-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-search-api-openapi.yml
- filename: trello-tokens-api-openapi.yml
  format: yaml
  label: trello Tokens API
  slug: trello-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-tokens-api-openapi.yml
- filename: trello-webhooks-api-openapi.yml
  format: yaml
  label: trello Webhooks API
  slug: trello-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trello Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trello secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Trello
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
