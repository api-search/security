---
api_key_in:
- header
api_specs:
- filename: churnkey-openapi.yml
  format: yaml
  label: Churnkey Data API
  slug: churnkey-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/churnkey/refs/heads/main/openapi/churnkey-openapi.yml
- filename: churnkey-openapi.yml
  format: yaml
  label: Churnkey Event Tracking API
  slug: churnkey-event-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/churnkey/refs/heads/main/openapi/churnkey-openapi.yml
- filename: churnkey-openapi.yml
  format: yaml
  label: Churnkey Billing Contact API
  slug: churnkey-billing-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/churnkey/refs/heads/main/openapi/churnkey-openapi.yml
- filename: churnkey-openapi.yml
  format: yaml
  label: Churnkey Data Subject Requests API
  slug: churnkey-data-subject-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/churnkey/refs/heads/main/openapi/churnkey-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Churnkey Authentication
name_suffix: Authentication
oauth_flows: []
overview: Churnkey secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Churnkey
provider_slug: churnkey
scheme_count: 2
schemes:
- description: Churnkey API key. The Data API (/v1/data) uses the Data API key from Settings > Account; the event and billing-contact endpoints (/v1/api) use a Churnkey API key.
  in: header
  name: apiKeyAuth
  parameter: x-ck-api-key
  sources:
  - openapi/churnkey-openapi.yml
  type: apiKey
- description: Churnkey Application ID (App ID) from Settings.
  in: header
  name: appIdAuth
  parameter: x-ck-app
  sources:
  - openapi/churnkey-openapi.yml
  type: apiKey
slug: churnkey-authentication
source_filename: churnkey-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/churnkey-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-ck-api-key\n  description: Churnkey API key. The Data API (/v1/data) uses the Data API key from Settings\n    > Account; the event and billing-contact endpoints (/v1/api) use a Churnkey API key.\n  sources:\n  - openapi/churnkey-openapi.yml\n- name: appIdAuth\n  type: apiKey\n  in: header\n  parameter: x-ck-app\n  description: Churnkey Application ID (App ID) from Settings.\n  sources:\n  - openapi/churnkey-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/churnkey/refs/heads/main/authentication/churnkey-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Churn Prevention
- Retention
- Cancellation Flows
- Failed Payment Recovery
- Dunning
- Reactivation
- Subscriptions
- SaaS
---
