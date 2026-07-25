---
api_key_in:
- header
api_specs:
- filename: talon-one-account-api-openapi.yml
  format: yaml
  label: Talon.One Account API
  slug: talon-one-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-account-api-openapi.yml
- filename: talon-one-applications-api-openapi.yml
  format: yaml
  label: Talon.One Applications API
  slug: talon-one-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-applications-api-openapi.yml
- filename: talon-one-attributes-api-openapi.yml
  format: yaml
  label: Talon.One Attributes API
  slug: talon-one-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-attributes-api-openapi.yml
- filename: talon-one-audiences-api-openapi.yml
  format: yaml
  label: Talon.One Audiences API
  slug: talon-one-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-audiences-api-openapi.yml
- filename: talon-one-campaigns-api-openapi.yml
  format: yaml
  label: Talon.One Campaigns API
  slug: talon-one-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-campaigns-api-openapi.yml
- filename: talon-one-collections-api-openapi.yml
  format: yaml
  label: Talon.One Collections API
  slug: talon-one-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-collections-api-openapi.yml
- filename: talon-one-coupons-api-openapi.yml
  format: yaml
  label: Talon.One Coupons API
  slug: talon-one-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-coupons-api-openapi.yml
- filename: talon-one-customer-profiles-api-openapi.yml
  format: yaml
  label: Talon.One Customer Profiles API
  slug: talon-one-customer-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-customer-profiles-api-openapi.yml
- filename: talon-one-customer-sessions-api-openapi.yml
  format: yaml
  label: Talon.One Customer Sessions API
  slug: talon-one-customer-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-customer-sessions-api-openapi.yml
- filename: talon-one-events-api-openapi.yml
  format: yaml
  label: Talon.One Events API
  slug: talon-one-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-events-api-openapi.yml
- filename: talon-one-exports-api-openapi.yml
  format: yaml
  label: Talon.One Exports API
  slug: talon-one-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-exports-api-openapi.yml
- filename: talon-one-loyalty-api-openapi.yml
  format: yaml
  label: Talon.One Loyalty API
  slug: talon-one-loyalty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-loyalty-api-openapi.yml
- filename: talon-one-referrals-api-openapi.yml
  format: yaml
  label: Talon.One Referrals API
  slug: talon-one-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/openapi/talon-one-referrals-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Talon One Authentication
name_suffix: Authentication
oauth_flows: []
overview: Talon.One secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Talon.One
provider_slug: talon-one
scheme_count: 1
schemes:
- description: 'Integration API key with the ApiKey-v1 prefix, e.g. header "Authorization: ApiKey-v1 <your-key>".'
  in: header
  name: integrationKey
  parameter: Authorization
  sources:
  - openapi/talon-one-openapi.yml
  type: apiKey
slug: talon-one-authentication
source_filename: talon-one-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/talon-one-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: integrationKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Integration API key with the ApiKey-v1 prefix, e.g. header \"Authorization: ApiKey-v1\n    <your-key>\".'\n  sources:\n  - openapi/talon-one-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talon-one/refs/heads/main/authentication/talon-one-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Promotions
- Loyalty
- Coupons
- Incentives
- Campaigns
- Personalization
- MarTech
- Rules Engine
---
