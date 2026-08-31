---
api_key_in: []
api_specs:
- filename: blues-wireless-alert-api-openapi.yml
  format: yaml
  label: Blues alert API
  slug: blues-wireless-alert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-alert-api-openapi.yml
- filename: blues-wireless-authorization-api-openapi.yml
  format: yaml
  label: Blues authorization API
  slug: blues-wireless-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-authorization-api-openapi.yml
- filename: blues-wireless-billing-account-api-openapi.yml
  format: yaml
  label: Blues billing_account API
  slug: blues-wireless-billing-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-billing-account-api-openapi.yml
- filename: blues-wireless-device-api-openapi.yml
  format: yaml
  label: Blues device API
  slug: blues-wireless-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-device-api-openapi.yml
- filename: blues-wireless-event-api-openapi.yml
  format: yaml
  label: Blues event API
  slug: blues-wireless-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-event-api-openapi.yml
- filename: blues-wireless-external-devices-api-openapi.yml
  format: yaml
  label: Blues external devices API
  slug: blues-wireless-external-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-external-devices-api-openapi.yml
- filename: blues-wireless-jobs-api-openapi.yml
  format: yaml
  label: Blues jobs API
  slug: blues-wireless-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-jobs-api-openapi.yml
- filename: blues-wireless-monitor-api-openapi.yml
  format: yaml
  label: Blues monitor API
  slug: blues-wireless-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-monitor-api-openapi.yml
- filename: blues-wireless-organization-api-openapi.yml
  format: yaml
  label: Blues organization API
  slug: blues-wireless-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-organization-api-openapi.yml
- filename: blues-wireless-project-api-openapi.yml
  format: yaml
  label: Blues project API
  slug: blues-wireless-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-project-api-openapi.yml
- filename: blues-wireless-route-api-openapi.yml
  format: yaml
  label: Blues route API
  slug: blues-wireless-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-route-api-openapi.yml
- filename: blues-wireless-usage-api-openapi.yml
  format: yaml
  label: Blues usage API
  slug: blues-wireless-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-usage-api-openapi.yml
- filename: blues-wireless-webhook-api-openapi.yml
  format: yaml
  label: Blues webhook API
  slug: blues-wireless-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/openapi/blues-wireless-webhook-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Blues Wireless Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blues secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Blues
provider_slug: blues-wireless
scheme_count: 1
schemes:
- description: Use a personal access token from notehub.io/api-access
  name: personalAccessToken
  scheme: bearer
  sources:
  - openapi/blues-wireless-notehub-api-openapi.yml
  type: http
slug: blues-wireless-authentication
source_filename: blues-wireless-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blues-wireless-notehub-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  description: Use a personal access token from notehub.io/api-access\n  sources:\n  - openapi/blues-wireless-notehub-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blues-wireless/refs/heads/main/authentication/blues-wireless-authentication.yml
summary_line: http · 1 scheme
tags:
- IoT
- Cellular
- Connectivity
- Device Management
- Fleet Management
- Satellite
- LoRa
- WiFi
- Notecard
- Notehub
---
