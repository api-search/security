---
api_key_in:
- header
api_specs:
- filename: watchguard-accounts-api-openapi.yml
  format: yaml
  label: WatchGuard Accounts API
  slug: watchguard-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-accounts-api-openapi.yml
- filename: watchguard-activations-api-openapi.yml
  format: yaml
  label: WatchGuard Activations API
  slug: watchguard-activations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-activations-api-openapi.yml
- filename: watchguard-allocations-api-openapi.yml
  format: yaml
  label: WatchGuard Allocations API
  slug: watchguard-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-allocations-api-openapi.yml
- filename: watchguard-authorization-api-openapi.yml
  format: yaml
  label: WatchGuard Authorization API
  slug: watchguard-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-authorization-api-openapi.yml
- filename: watchguard-configurations-api-openapi.yml
  format: yaml
  label: WatchGuard Configurations API
  slug: watchguard-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-configurations-api-openapi.yml
- filename: watchguard-device-actions-api-openapi.yml
  format: yaml
  label: WatchGuard Device Actions API
  slug: watchguard-device-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-device-actions-api-openapi.yml
- filename: watchguard-devices-api-openapi.yml
  format: yaml
  label: WatchGuard Devices API
  slug: watchguard-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-devices-api-openapi.yml
- filename: watchguard-licenses-api-openapi.yml
  format: yaml
  label: WatchGuard Licenses API
  slug: watchguard-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-licenses-api-openapi.yml
- filename: watchguard-operators-api-openapi.yml
  format: yaml
  label: WatchGuard Operators API
  slug: watchguard-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-operators-api-openapi.yml
- filename: watchguard-risk-assessment-api-openapi.yml
  format: yaml
  label: WatchGuard Risk Assessment API
  slug: watchguard-risk-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-risk-assessment-api-openapi.yml
- filename: watchguard-security-events-api-openapi.yml
  format: yaml
  label: WatchGuard Security Events API
  slug: watchguard-security-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/openapi/watchguard-security-events-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Watchguard Authentication
name_suffix: Authentication
oauth_flows: []
overview: WatchGuard secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WatchGuard
provider_slug: watchguard
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained from the WatchGuard Authentication API.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/watchguard-cloud-platform-openapi.yml
  - openapi/watchguard-endpoint-security-openapi.yml
  type: http
- description: API key from the WatchGuard Cloud Managed Access page.
  in: header
  name: apiKeyAuth
  parameter: WatchGuard-API-Key
  sources:
  - openapi/watchguard-cloud-platform-openapi.yml
  - openapi/watchguard-endpoint-security-openapi.yml
  type: apiKey
slug: watchguard-authentication
source_filename: watchguard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/watchguard-cloud-platform-openapi.yml, openapi/watchguard-endpoint-security-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained from the WatchGuard Authentication API.\n  sources:\n  - openapi/watchguard-cloud-platform-openapi.yml\n  - openapi/watchguard-endpoint-security-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: WatchGuard-API-Key\n  description: API key from the WatchGuard Cloud Managed Access page.\n  sources:\n  - openapi/watchguard-cloud-platform-openapi.yml\n  - openapi/watchguard-endpoint-security-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/watchguard/refs/heads/main/authentication/watchguard-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Cloud Security
- Endpoint Security
- Firewall
- MFA
- Network Security
- Zero Trust
---
