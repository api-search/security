---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: johnson-controls-activities-api-openapi.yml
  format: yaml
  label: Johnson Controls Activities API
  slug: johnson-controls-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-activities-api-openapi.yml
- filename: johnson-controls-alarms-api-openapi.yml
  format: yaml
  label: Johnson Controls Alarms API
  slug: johnson-controls-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-alarms-api-openapi.yml
- filename: johnson-controls-audits-api-openapi.yml
  format: yaml
  label: Johnson Controls Audits API
  slug: johnson-controls-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-audits-api-openapi.yml
- filename: johnson-controls-authentication-api-openapi.yml
  format: yaml
  label: Johnson Controls Authentication API
  slug: johnson-controls-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-authentication-api-openapi.yml
- filename: johnson-controls-equipment-api-openapi.yml
  format: yaml
  label: Johnson Controls Equipment API
  slug: johnson-controls-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-equipment-api-openapi.yml
- filename: johnson-controls-network-devices-api-openapi.yml
  format: yaml
  label: Johnson Controls network devices API
  slug: johnson-controls-network-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-network-devices-api-openapi.yml
- filename: johnson-controls-objects-api-openapi.yml
  format: yaml
  label: Johnson Controls Objects API
  slug: johnson-controls-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-objects-api-openapi.yml
- filename: johnson-controls-schemas-api-openapi.yml
  format: yaml
  label: Johnson Controls Schemas API
  slug: johnson-controls-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-schemas-api-openapi.yml
- filename: johnson-controls-spaces-api-openapi.yml
  format: yaml
  label: Johnson Controls Spaces API
  slug: johnson-controls-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-spaces-api-openapi.yml
- filename: johnson-controls-streaming-api-openapi.yml
  format: yaml
  label: Johnson Controls Streaming API
  slug: johnson-controls-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-streaming-api-openapi.yml
- filename: johnson-controls-time-series-api-openapi.yml
  format: yaml
  label: Johnson Controls time series API
  slug: johnson-controls-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/openapi/johnson-controls-time-series-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Johnson Controls Authentication
name_suffix: Authentication
oauth_flows: []
overview: Johnson Controls secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Johnson Controls
provider_slug: johnson-controls
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'Most of the calls in the API use bearer token authentication. What this

    means is that these requests require an `Authorization` header to be set to

    a value with the following format: `Bearer: {accessToken}`. Use the

    [`/login`](#operation/createToken) operation to request an `accessToken`. An

    example of the full header would look like the following:

    `Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOi'
  name: Bearer-Authentication
  scheme: bearer
  sources:
  - openapi/johnson-controls-metasys-openapi.yml
  type: http
- description: 'The [Streaming operation](#operation/getStream) is the only operation to use

    API key authentication, because web browsers do not allow setting custom

    headers when initiating Server Sent Event connections.'
  in: query
  name: API-Key-Authentication
  parameter: access_token
  sources:
  - openapi/johnson-controls-metasys-openapi.yml
  type: apiKey
slug: johnson-controls-authentication
source_filename: johnson-controls-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/johnson-controls-metasys-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: Bearer-Authentication\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Most of the calls in the API use bearer token authentication. What this\n    means is that these requests require an `Authorization` header to be set to\n    a value with the following format: `Bearer: {accessToken}`. Use the\n    [`/login`](#operation/createToken) operation to request an `accessToken`. An\n    example of the full header would look like the following:\n    `Authorization: Bearer eyJ0eXAiOiJKV1QiLCJhbGciOi\n  sources:\n  - openapi/johnson-controls-metasys-openapi.yml\n- name: API-Key-Authentication\n  type: apiKey\n  in: query\n  parameter: access_token\n  description: |-\n    The [Streaming operation](#operation/getStream) is the only operation to use\n    API key authentication, because\
  \ web browsers do not allow setting custom\n    headers when initiating Server Sent Event connections.\n  sources:\n  - openapi/johnson-controls-metasys-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/authentication/johnson-controls-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Building Automation
- Energy Storage
- Fire & Security
- HVAC
- Smart Buildings
- Fortune 100
---
