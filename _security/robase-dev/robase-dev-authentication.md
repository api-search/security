---
anonymous_access: false
api_key_in: []
api_specs:
- filename: robase-dev-dashboard-api-openapi.yml
  format: yaml
  label: robase-dev Dashboard API
  slug: robase-dev-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-dashboard-api-openapi.yml
- filename: robase-dev-otp-api-openapi.yml
  format: yaml
  label: robase-dev OTP API
  slug: robase-dev-otp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-otp-api-openapi.yml
- filename: robase-dev-sms-api-openapi.yml
  format: yaml
  label: robase-dev SMS API
  slug: robase-dev-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-sms-api-openapi.yml
- filename: robase-dev-system-api-openapi.yml
  format: yaml
  label: robase-dev System API
  slug: robase-dev-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-system-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Robase Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: robase-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: robase-dev
provider_slug: robase-dev
scheme_count: 1
schemes:
- bearerFormat: robe_<64-hex>
  description: API keys are Bearer tokens. Live keys start with robe_ plus 64 hex characters. Agent keys start with robe_agent_
  scheme: bearer
  type: http
slug: robase-dev-authentication
source_filename: robase-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: \"https://docs.robase.dev/api-reference/authentication.md\"\nschemes:\n  - type: \"http\"\n    scheme: \"bearer\"\n    bearerFormat: \"robe_<64-hex>\"\n    description: \"API keys are Bearer tokens. Live keys start with robe_ plus 64 hex characters. Agent keys start with robe_agent_\"\n"
source_yaml_url: https://artifacts.apis.io/robase-dev/authentication/robase-dev-authentication.yml
summary_line: 1 scheme
tags:
- SMS
- OTP
- Africa
- Messaging
- API
- Communications
---
