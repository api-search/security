---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: krobar-ai-admin-api-openapi.yml
  format: yaml
  label: Krobar.ai Admin API
  slug: krobar-ai-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-admin-api-openapi.yml
- filename: krobar-ai-admin-plans-api-openapi.yml
  format: yaml
  label: Krobar.ai Admin Plans API
  slug: krobar-ai-admin-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-admin-plans-api-openapi.yml
- filename: krobar-ai-attachments-api-openapi.yml
  format: yaml
  label: Krobar.ai Attachments API
  slug: krobar-ai-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-attachments-api-openapi.yml
- filename: krobar-ai-authentication-api-openapi.yml
  format: yaml
  label: Krobar.ai Authentication API
  slug: krobar-ai-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-authentication-api-openapi.yml
- filename: krobar-ai-conversations-api-openapi.yml
  format: yaml
  label: Krobar.ai Conversations API
  slug: krobar-ai-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-conversations-api-openapi.yml
- filename: krobar-ai-data-sources-api-openapi.yml
  format: yaml
  label: Krobar.ai Data Sources API
  slug: krobar-ai-data-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-data-sources-api-openapi.yml
- filename: krobar-ai-distributions-api-openapi.yml
  format: yaml
  label: Krobar.ai Distributions API
  slug: krobar-ai-distributions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-distributions-api-openapi.yml
- filename: krobar-ai-email-api-openapi.yml
  format: yaml
  label: Krobar.ai Email API
  slug: krobar-ai-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-email-api-openapi.yml
- filename: krobar-ai-formulas-api-openapi.yml
  format: yaml
  label: Krobar.ai Formulas API
  slug: krobar-ai-formulas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-formulas-api-openapi.yml
- filename: krobar-ai-graphs-api-openapi.yml
  format: yaml
  label: Krobar.ai Graphs API
  slug: krobar-ai-graphs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-graphs-api-openapi.yml
- filename: krobar-ai-health-api-openapi.yml
  format: yaml
  label: Krobar.ai Health API
  slug: krobar-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-health-api-openapi.yml
- filename: krobar-ai-invite-tokens-api-openapi.yml
  format: yaml
  label: Krobar.ai Invite Tokens API
  slug: krobar-ai-invite-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-invite-tokens-api-openapi.yml
- filename: krobar-ai-mailchimp-api-openapi.yml
  format: yaml
  label: Krobar.ai Mailchimp API
  slug: krobar-ai-mailchimp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-mailchimp-api-openapi.yml
- filename: krobar-ai-me-api-openapi.yml
  format: yaml
  label: Krobar.ai Me API
  slug: krobar-ai-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-me-api-openapi.yml
- filename: krobar-ai-plans-api-openapi.yml
  format: yaml
  label: Krobar.ai Plans API
  slug: krobar-ai-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-plans-api-openapi.yml
- filename: krobar-ai-policies-api-openapi.yml
  format: yaml
  label: Krobar.ai Policies API
  slug: krobar-ai-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-policies-api-openapi.yml
- filename: krobar-ai-projects-api-openapi.yml
  format: yaml
  label: Krobar.ai Projects API
  slug: krobar-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-projects-api-openapi.yml
- filename: krobar-ai-task-templates-api-openapi.yml
  format: yaml
  label: Krobar.ai Task Templates API
  slug: krobar-ai-task-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-task-templates-api-openapi.yml
- filename: krobar-ai-teams-api-openapi.yml
  format: yaml
  label: Krobar.ai Teams API
  slug: krobar-ai-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-teams-api-openapi.yml
- filename: krobar-ai-templates-api-openapi.yml
  format: yaml
  label: Krobar.ai Templates API
  slug: krobar-ai-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-templates-api-openapi.yml
- filename: krobar-ai-users-api-openapi.yml
  format: yaml
  label: Krobar.ai Users API
  slug: krobar-ai-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/krobar-ai/openapi/krobar-ai-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Krobar.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Krobar.ai secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Krobar.ai
provider_slug: krobar-ai
scheme_count: 2
schemes:
- in: cookie
  name: APIKeyCookie
  parameter: access_token
  sources:
  - openapi/krobar-ai-openapi.json
  type: apiKey
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/krobar-ai-openapi.json
  type: apiKey
slug: krobar-ai-authentication
source_filename: krobar-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: derived\nsource: openapi/krobar-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: APIKeyCookie\n  type: apiKey\n  in: cookie\n  parameter: access_token\n  sources:\n  - openapi/krobar-ai-openapi.json\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/krobar-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/krobar-ai/authentication/krobar-ai-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Artificial Intelligence
- Forecasting
- Business
- Analytics
- Modeling
---
