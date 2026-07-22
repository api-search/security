---
api_key_in:
- query
- header
- body
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Swipeguide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swipeguide secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Swipeguide
provider_slug: swipeguide
scheme_count: 3
schemes:
- description: API key supplied as the `auth` query parameter.
  in: query
  name: apiKeyQuery
  parameter: auth
  type: apiKey
- description: API key supplied in the `L2LAUTH` HTTP header.
  in: header
  name: apiKeyHeader
  parameter: L2LAUTH
  type: apiKey
- description: API key supplied as `auth` in the POST request body.
  in: body
  name: apiKeyBody
  parameter: auth
  type: apiKey
slug: swipeguide-authentication
source_filename: swipeguide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://support.leading2lean.com/hc/en-us/articles/360051148492-API-Documentation\ndocs: https://support.leading2lean.com/hc/en-us/articles/360051148492-API-Documentation\nsummary:\n  types: [apiKey]\n  api_key_in: [query, header, body]\n  request_signing: hmac-sha512\n  oauth2_flows: []\nnotes: >-\n  The L2L Dispatch API authenticates every HTTPS request with an API Key. API\n  Keys are created exclusively by L2L Support for an API user account (contact\n  support@leading2lean.com). For sensitive operations a separate Secret Key can\n  sign requests using HMAC-SHA512 to guarantee they were not tampered with.\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: auth\n  description: API key supplied as the `auth` query parameter.\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: L2LAUTH\n  description: API key supplied in the `L2LAUTH` HTTP header.\n- name: apiKeyBody\n  type: apiKey\n  in:\
  \ body\n  parameter: auth\n  description: API key supplied as `auth` in the POST request body.\nrequest_signing:\n  algorithm: HMAC-SHA512\n  key: secret-key\n  scope: sensitive operations\n  description: >-\n    Optional request signing using a Secret Key (distinct from the API Key) to\n    verify request integrity for sensitive operations.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swipeguide/refs/heads/main/authentication/swipeguide-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Manufacturing
- Work Instructions
- Frontline
- Shop Floor
- Maintenance
- Connected Worker
- Smart Manufacturing
- Industrial
---
