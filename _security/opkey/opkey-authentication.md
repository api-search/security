---
api_key_in:
- header
api_specs:
- filename: opkey-apk-instrumentation-api-openapi.yml
  format: yaml
  label: Opkey Apk Instrumentation API
  slug: opkey-apk-instrumentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-apk-instrumentation-api-openapi.yml
- filename: opkey-apk-instrumentation-apis-api-openapi.yml
  format: yaml
  label: Opkey Apk Instrumentation Apis API
  slug: opkey-apk-instrumentation-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-apk-instrumentation-apis-api-openapi.yml
- filename: opkey-app-center-api-api-openapi.yml
  format: yaml
  label: Opkey App Center Api API
  slug: opkey-app-center-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-app-center-api-api-openapi.yml
- filename: opkey-app-control-api-openapi.yml
  format: yaml
  label: Opkey App Control API
  slug: opkey-app-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-app-control-api-openapi.yml
- filename: opkey-appium-automation-api-openapi.yml
  format: yaml
  label: Opkey Appium Automation API
  slug: opkey-appium-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-appium-automation-api-openapi.yml
- filename: opkey-authentication-api-openapi.yml
  format: yaml
  label: Opkey Authentication API
  slug: opkey-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-authentication-api-openapi.yml
- filename: opkey-device-booking-session-api-openapi.yml
  format: yaml
  label: Opkey Device Booking & Session API
  slug: opkey-device-booking-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-device-booking-session-api-openapi.yml
- filename: opkey-device-interaction-api-openapi.yml
  format: yaml
  label: Opkey Device Interaction API
  slug: opkey-device-interaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-device-interaction-api-openapi.yml
- filename: opkey-file-management-api-openapi.yml
  format: yaml
  label: Opkey File Management API
  slug: opkey-file-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-file-management-api-openapi.yml
- filename: opkey-generic-api-openapi.yml
  format: yaml
  label: Opkey Generic API
  slug: opkey-generic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-generic-api-openapi.yml
- filename: opkey-network-simulation-api-openapi.yml
  format: yaml
  label: Opkey Network Simulation API
  slug: opkey-network-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-network-simulation-api-openapi.yml
- filename: opkey-performance-api-openapi.yml
  format: yaml
  label: Opkey Performance API
  slug: opkey-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-performance-api-openapi.yml
- filename: opkey-resigning-apis-api-openapi.yml
  format: yaml
  label: Opkey Resigning Apis API
  slug: opkey-resigning-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-resigning-apis-api-openapi.yml
- filename: opkey-session-media-logs-api-openapi.yml
  format: yaml
  label: Opkey Session Media & Logs API
  slug: opkey-session-media-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-session-media-logs-api-openapi.yml
- filename: opkey-xctest-automation-api-openapi.yml
  format: yaml
  label: Opkey Xctest Automation API
  slug: opkey-xctest-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/openapi/opkey-xctest-automation-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Opkey Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opkey secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Opkey
provider_slug: opkey
scheme_count: 2
schemes:
- description: HTTP Basic with your pCloudy email as the username and your API access key as the password. Used only by GET /api/access to mint an access token.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/opkey-pcloudy-openapi.yml
  type: http
- description: Access token returned by GET /api/access. Newer /api/v2/* operations send it as a `token` header; several legacy /api/* operations send the same token as a `token` field in the JSON request body.
  in: header
  name: accessToken
  parameter: token
  sources:
  - openapi/opkey-pcloudy-openapi.yml
  type: apiKey
slug: opkey-authentication
source_filename: opkey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: openapi/opkey-pcloudy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with your pCloudy email as the username and your API access key as\n    the password. Used only by GET /api/access to mint an access token.\n  sources:\n  - openapi/opkey-pcloudy-openapi.yml\n- name: accessToken\n  type: apiKey\n  in: header\n  parameter: token\n  description: Access token returned by GET /api/access. Newer /api/v2/* operations send it\n    as a `token` header; several legacy /api/* operations send the same token as a `token` field\n    in the JSON request body.\n  sources:\n  - openapi/opkey-pcloudy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opkey/refs/heads/main/authentication/opkey-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Testing
- Test Automation
- Quality Assurance
- DevOps
- Continuous Integration
- Mobile Testing
- Device Cloud
- ERP
- Artificial Intelligence
- Agents
- MCP
---
