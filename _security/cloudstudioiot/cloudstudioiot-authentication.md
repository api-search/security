---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: cloudstudioiot-access-tokens-api-openapi.yml
  format: yaml
  label: Cloud Studio IoT Access tokens API
  slug: cloudstudioiot-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudstudioiot/refs/heads/main/openapi/cloudstudioiot-access-tokens-api-openapi.yml
- filename: cloudstudioiot-alarms-api-openapi.yml
  format: yaml
  label: Cloud Studio IoT Alarms API
  slug: cloudstudioiot-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudstudioiot/refs/heads/main/openapi/cloudstudioiot-alarms-api-openapi.yml
- filename: cloudstudioiot-alerts-api-openapi.yml
  format: yaml
  label: Cloud Studio IoT Alerts API
  slug: cloudstudioiot-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudstudioiot/refs/heads/main/openapi/cloudstudioiot-alerts-api-openapi.yml
- filename: cloudstudioiot-endpoint-data-api-openapi.yml
  format: yaml
  label: Cloud Studio IoT Endpoint data API
  slug: cloudstudioiot-endpoint-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudstudioiot/refs/heads/main/openapi/cloudstudioiot-endpoint-data-api-openapi.yml
- filename: cloudstudioiot-geozones-api-openapi.yml
  format: yaml
  label: Cloud Studio IoT Geozones API
  slug: cloudstudioiot-geozones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudstudioiot/refs/heads/main/openapi/cloudstudioiot-geozones-api-openapi.yml
- filename: cloudstudioiot-instance-api-openapi.yml
  format: yaml
  label: Cloud Studio IoT Instance API
  slug: cloudstudioiot-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudstudioiot/refs/heads/main/openapi/cloudstudioiot-instance-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Cloudstudioiot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloud Studio IoT secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cloud Studio IoT
provider_slug: cloudstudioiot
scheme_count: 2
schemes:
- description: 'Persistent access token sent as `Authorization: Bearer {accessToken}`.'
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/cloudstudioiot-openapi.yaml
  type: http
- description: The same access token in the query string, for clients that cannot set headers.
  in: query
  name: accessTokenQuery
  parameter: accessToken
  sources:
  - openapi/cloudstudioiot-openapi.yaml
  type: apiKey
slug: cloudstudioiot-authentication
source_filename: cloudstudioiot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: derived\nsource: openapi/cloudstudioiot-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: 'Persistent access token sent as `Authorization: Bearer {accessToken}`.'\n  sources:\n  - openapi/cloudstudioiot-openapi.yaml\n- name: accessTokenQuery\n  type: apiKey\n  in: query\n  parameter: accessToken\n  description: The same access token in the query string, for clients that cannot set headers.\n  sources:\n  - openapi/cloudstudioiot-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudstudioiot/refs/heads/main/authentication/cloudstudioiot-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- IoT
- AI
- Industrial
- Platform
---
