---
api_key_in: []
api_specs:
- filename: shuftipro-openapi.yml
  format: yaml
  label: Shufti Pro Verification API
  slug: shuftipro-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuftipro/refs/heads/main/openapi/shuftipro-openapi.yml
- filename: shuftipro-openapi.yml
  format: yaml
  label: Shufti Pro KYB API
  slug: shuftipro-kyb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuftipro/refs/heads/main/openapi/shuftipro-openapi.yml
- filename: shuftipro-openapi.yml
  format: yaml
  label: Shufti Pro AML & Background Checks API
  slug: shuftipro-aml-background-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuftipro/refs/heads/main/openapi/shuftipro-openapi.yml
- filename: shuftipro-openapi.yml
  format: yaml
  label: Shufti Pro Status API
  slug: shuftipro-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuftipro/refs/heads/main/openapi/shuftipro-openapi.yml
- filename: shuftipro-openapi.yml
  format: yaml
  label: Shufti Pro Webhooks API
  slug: shuftipro-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shuftipro/refs/heads/main/openapi/shuftipro-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Shuftipro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shufti Pro secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Shufti Pro
provider_slug: shuftipro
scheme_count: 2
schemes:
- description: HTTP Basic Auth using your Client ID as the username and your Secret Key as the password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/shuftipro-openapi.yml
  type: http
- description: Bearer access token shared with the client; valid for 10 minutes and single use.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/shuftipro-openapi.yml
  type: http
slug: shuftipro-authentication
source_filename: shuftipro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shuftipro-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using your Client ID as the username and your Secret Key as the\n    password.\n  sources:\n  - openapi/shuftipro-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer access token shared with the client; valid for 10 minutes and single use.\n  sources:\n  - openapi/shuftipro-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shuftipro/refs/heads/main/authentication/shuftipro-authentication.yml
summary_line: http · 2 schemes
tags:
- Identity Verification
- KYC
- KYB
- AML
- Compliance
---
