---
api_key_in:
- header
- query
api_specs:
- filename: adafruit-io-activities-api-openapi.yml
  format: yaml
  label: Adafruit IO Activities API
  slug: adafruit-io-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-activities-api-openapi.yml
- filename: adafruit-io-blocks-api-openapi.yml
  format: yaml
  label: Adafruit IO Blocks API
  slug: adafruit-io-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-blocks-api-openapi.yml
- filename: adafruit-io-dashboards-api-openapi.yml
  format: yaml
  label: Adafruit IO Dashboards API
  slug: adafruit-io-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-dashboards-api-openapi.yml
- filename: adafruit-io-data-api-openapi.yml
  format: yaml
  label: Adafruit IO Data API
  slug: adafruit-io-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-data-api-openapi.yml
- filename: adafruit-io-feeds-api-openapi.yml
  format: yaml
  label: Adafruit IO Feeds API
  slug: adafruit-io-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-feeds-api-openapi.yml
- filename: adafruit-io-groups-api-openapi.yml
  format: yaml
  label: Adafruit IO Groups API
  slug: adafruit-io-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-groups-api-openapi.yml
- filename: adafruit-io-permissions-api-openapi.yml
  format: yaml
  label: Adafruit IO Permissions API
  slug: adafruit-io-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-permissions-api-openapi.yml
- filename: adafruit-io-tokens-api-openapi.yml
  format: yaml
  label: Adafruit IO Tokens API
  slug: adafruit-io-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-tokens-api-openapi.yml
- filename: adafruit-io-triggers-api-openapi.yml
  format: yaml
  label: Adafruit IO Triggers API
  slug: adafruit-io-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-triggers-api-openapi.yml
- filename: adafruit-io-users-api-openapi.yml
  format: yaml
  label: Adafruit IO Users API
  slug: adafruit-io-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-users-api-openapi.yml
- filename: adafruit-io-webhooks-api-openapi.yml
  format: yaml
  label: Adafruit IO Webhooks API
  slug: adafruit-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/openapi/adafruit-io-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Adafruit Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adafruit IO secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Adafruit IO
provider_slug: adafruit-io
scheme_count: 3
schemes:
- description: The AIO Key is used to restrict or grant access to your data. The key is unique, and you can generate a key per feed, and control it in many different ways. The easiest process is to just use your automatically generated master key. You can access this key right from the right-hand side of your dashboard or from an individual feed page.
  in: header
  name: HeaderKey
  parameter: X-AIO-Key
  sources:
  - openapi/adafruit-io-rest-api-openapi.yml
  type: apiKey
- description: The AIO Key is used to restrict or grant access to your data. The key is unique, and you can generate a key per feed, and control it in many different ways. The easiest process is to just use your automatically generated master key. You can access this key right from the right-hand side of your dashboard or from an individual feed page.
  in: query
  name: QueryKey
  parameter: X-AIO-Key
  sources:
  - openapi/adafruit-io-rest-api-openapi.yml
  type: apiKey
- description: The AIO Signature is an AWS inspired request signature.
  in: header
  name: HeaderSignature
  parameter: X-AIO-Signature
  sources:
  - openapi/adafruit-io-rest-api-openapi.yml
  type: apiKey
slug: adafruit-io-authentication
source_filename: adafruit-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adafruit-io-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: HeaderKey\n  type: apiKey\n  in: header\n  parameter: X-AIO-Key\n  description: The AIO Key is used to restrict or grant access to your data. The key is unique,\n    and you can generate a key per feed, and control it in many different ways. The easiest\n    process is to just use your automatically generated master key. You can access this key\n    right from the right-hand side of your dashboard or from an individual feed page.\n  sources:\n  - openapi/adafruit-io-rest-api-openapi.yml\n- name: QueryKey\n  type: apiKey\n  in: query\n  parameter: X-AIO-Key\n  description: The AIO Key is used to restrict or grant access to your data. The key is unique,\n    and you can generate a key per feed, and control it in many different ways. The easiest\n    process is to just use your automatically generated\
  \ master key. You can access this key\n    right from the right-hand side of your dashboard or from an individual feed page.\n  sources:\n  - openapi/adafruit-io-rest-api-openapi.yml\n- name: HeaderSignature\n  type: apiKey\n  in: header\n  parameter: X-AIO-Signature\n  description: The AIO Signature is an AWS inspired request signature.\n  sources:\n  - openapi/adafruit-io-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adafruit-io/refs/heads/main/authentication/adafruit-io-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- IoT
- Internet of Things
- MQTT
- Maker
- Hobbyist
- CircuitPython
- Arduino
- ESP32
- Feather
- Dashboards
- Time Series
---
