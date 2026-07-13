---
api_key_in:
- header
api_specs:
- filename: freshworks-freshdesk-api-openapi.yml
  format: yaml
  label: Freshworks Freshdesk API
  slug: freshdesk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/openapi/freshworks-freshdesk-api-openapi.yml
- filename: freshworks-freshservice-api-openapi.yml
  format: yaml
  label: Freshworks Freshservice API
  slug: freshservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/openapi/freshworks-freshservice-api-openapi.yml
- filename: freshworks-freshsales-api-openapi.yml
  format: yaml
  label: Freshworks Freshsales API
  slug: freshsales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/openapi/freshworks-freshsales-api-openapi.yml
- filename: freshworks-freshchat-api-openapi.yml
  format: yaml
  label: Freshworks Freshchat API
  slug: freshchat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/openapi/freshworks-freshchat-api-openapi.yml
- filename: freshworks-freshcaller-api-openapi.yml
  format: yaml
  label: Freshworks Freshcaller API
  slug: freshcaller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/openapi/freshworks-freshcaller-api-openapi.yml
- filename: freshworks-freshteam-api-openapi.yml
  format: yaml
  label: Freshworks Freshteam API
  slug: freshteam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/openapi/freshworks-freshteam-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Freshworks Authentication
name_suffix: Authentication
oauth_flows: []
overview: freshworks secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: freshworks
provider_slug: freshworks
scheme_count: 4
schemes:
- description: API key authentication. The API key can be found in your Freshcaller admin settings.
  in: header
  name: apiKeyAuth
  parameter: X-Api-Auth
  sources:
  - openapi/freshworks-freshcaller-api-openapi.yml
  type: apiKey
- description: Bearer token authentication. Obtain the API token from the Freshchat admin settings panel.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/freshworks-freshchat-api-openapi.yml
  - openapi/freshworks-freshteam-api-openapi.yml
  type: http
- description: Use your API key as the username and X as the password. The API key can be found in your Freshdesk profile settings.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/freshworks-freshdesk-api-openapi.yml
  - openapi/freshworks-freshservice-api-openapi.yml
  type: http
- description: Token-based authentication. Use the format "Token token=your_api_key".
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/freshworks-freshsales-api-openapi.yml
  type: apiKey
slug: freshworks-authentication
source_filename: freshworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freshworks-freshcaller-api-openapi.yml, openapi/freshworks-freshchat-api-openapi.yml,\n  openapi/freshworks-freshdesk-api-openapi.yml, openapi/freshworks-freshsales-api-openapi.yml,\n  openapi/freshworks-freshservice-api-openapi.yml, openapi/freshworks-freshteam-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Auth\n  description: API key authentication. The API key can be found in your Freshcaller admin settings.\n  sources:\n  - openapi/freshworks-freshcaller-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication. Obtain the API token from the Freshchat admin settings\n    panel.\n  sources:\n  - openapi/freshworks-freshchat-api-openapi.yml\n  - openapi/freshworks-freshteam-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description:\
  \ Use your API key as the username and X as the password. The API key can be found\n    in your Freshdesk profile settings.\n  sources:\n  - openapi/freshworks-freshdesk-api-openapi.yml\n  - openapi/freshworks-freshservice-api-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Token-based authentication. Use the format \"Token token=your_api_key\".\n  sources:\n  - openapi/freshworks-freshsales-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/authentication/freshworks-authentication.yml
summary_line: apiKey/http · 4 schemes
tags: []
---
