---
api_key_in:
- header
api_specs:
- filename: codat-platform-openapi.json
  format: json
  label: Codat Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat/refs/heads/main/openapi/codat-platform-openapi.json
- filename: codat-lending-openapi.json
  format: json
  label: Codat Lending API
  slug: lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat/refs/heads/main/openapi/codat-lending-openapi.json
- filename: codat-bank-feeds-openapi.json
  format: json
  label: Codat Bank Feeds API
  slug: bank-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codat/refs/heads/main/openapi/codat-bank-feeds-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Codat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Codat secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Codat
provider_slug: codat
scheme_count: 1
schemes:
- description: The word "Basic" followed by a space and your API key. [API keys](https://docs.codat.io/platform-api#/schemas/ApiKeyDetails) are tokens used to control access to the API. You can get an API key via [the Codat Portal](https://app.codat.io/developers/api-keys), via [the API](https://docs.codat.io/platform-api#/operations/list-api-keys), or [read more](https://docs.codat.io/using-the-api/authenticati
  in: header
  name: auth_header
  parameter: Authorization
  sources:
  - openapi/codat-bank-feeds-openapi.json
  - openapi/codat-lending-openapi.json
  - openapi/codat-platform-openapi.json
  type: apiKey
slug: codat-authentication
source_filename: codat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/codat-bank-feeds-openapi.json, openapi/codat-lending-openapi.json, openapi/codat-platform-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: auth_header\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: The word \"Basic\" followed by a space and your API key. [API keys](https://docs.codat.io/platform-api#/schemas/ApiKeyDetails)\n    are tokens used to control access to the API. You can get an API key via [the Codat Portal](https://app.codat.io/developers/api-keys),\n    via [the API](https://docs.codat.io/platform-api#/operations/list-api-keys), or [read more](https://docs.codat.io/using-the-api/authenticati\n  sources:\n  - openapi/codat-bank-feeds-openapi.json\n  - openapi/codat-lending-openapi.json\n  - openapi/codat-platform-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codat/refs/heads/main/authentication/codat-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Unified_API
---
