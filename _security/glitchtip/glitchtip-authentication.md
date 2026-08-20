---
api_key_in:
- cookie
api_specs:
- filename: glitchtip-accept-api-openapi.yml
  format: yaml
  label: GlitchTip Accept API
  slug: glitchtip-accept-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-accept-api-openapi.yml
- filename: glitchtip-api-tokens-api-openapi.yml
  format: yaml
  label: GlitchTip Api Tokens API
  slug: glitchtip-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-api-tokens-api-openapi.yml
- filename: glitchtip-embed-api-openapi.yml
  format: yaml
  label: GlitchTip Embed API
  slug: glitchtip-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-embed-api-openapi.yml
- filename: glitchtip-generate-recovery-codes-api-openapi.yml
  format: yaml
  label: GlitchTip Generate Recovery Codes API
  slug: glitchtip-generate-recovery-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-generate-recovery-codes-api-openapi.yml
- filename: glitchtip-glitchtip-api-api-openapi.yml
  format: yaml
  label: GlitchTip GlitchTip API API
  slug: glitchtip-glitchtip-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-glitchtip-api-api-openapi.yml
- filename: glitchtip-import-api-openapi.yml
  format: yaml
  label: GlitchTip Import API
  slug: glitchtip-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-import-api-openapi.yml
- filename: glitchtip-instance-license-api-openapi.yml
  format: yaml
  label: GlitchTip Instance License API
  slug: glitchtip-instance-license-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-instance-license-api-openapi.yml
- filename: glitchtip-issues-api-openapi.yml
  format: yaml
  label: GlitchTip Issues API
  slug: glitchtip-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-issues-api-openapi.yml
- filename: glitchtip-organizations-api-openapi.yml
  format: yaml
  label: GlitchTip Organizations API
  slug: glitchtip-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-organizations-api-openapi.yml
- filename: glitchtip-projects-api-openapi.yml
  format: yaml
  label: GlitchTip Projects API
  slug: glitchtip-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-projects-api-openapi.yml
- filename: glitchtip-security-api-openapi.yml
  format: yaml
  label: GlitchTip Security API
  slug: glitchtip-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-security-api-openapi.yml
- filename: glitchtip-settings-api-openapi.yml
  format: yaml
  label: GlitchTip Settings API
  slug: glitchtip-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-settings-api-openapi.yml
- filename: glitchtip-store-api-openapi.yml
  format: yaml
  label: GlitchTip Store API
  slug: glitchtip-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-store-api-openapi.yml
- filename: glitchtip-stripe-api-openapi.yml
  format: yaml
  label: GlitchTip Stripe API
  slug: glitchtip-stripe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-stripe-api-openapi.yml
- filename: glitchtip-teams-api-openapi.yml
  format: yaml
  label: GlitchTip Teams API
  slug: glitchtip-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-teams-api-openapi.yml
- filename: glitchtip-users-api-openapi.yml
  format: yaml
  label: GlitchTip Users API
  slug: glitchtip-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-users-api-openapi.yml
- filename: glitchtip-wizard-api-openapi.yml
  format: yaml
  label: GlitchTip Wizard API
  slug: glitchtip-wizard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-wizard-api-openapi.yml
- filename: glitchtip-wizard-set-token-api-openapi.yml
  format: yaml
  label: GlitchTip Wizard Set Token API
  slug: glitchtip-wizard-set-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/openapi/glitchtip-wizard-set-token-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Glitchtip Authentication
name_suffix: Authentication
oauth_flows: []
overview: GlitchTip secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GlitchTip
provider_slug: glitchtip
scheme_count: 2
schemes:
- name: TokenAuth
  scheme: bearer
  sources:
  - openapi/glitchtip-rest-openapi.yml
  type: http
- in: cookie
  name: SessionAuth
  parameter: sessionid
  sources:
  - openapi/glitchtip-rest-openapi.yml
  type: apiKey
slug: glitchtip-authentication
source_filename: glitchtip-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/glitchtip-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: TokenAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/glitchtip-rest-openapi.yml\n- name: SessionAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/glitchtip-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/authentication/glitchtip-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Error Tracking
- Performance Monitoring
- Uptime Monitoring
- Application Monitoring
- Open-Source
- Sentry Compatible
- Observability
- Logging
---
