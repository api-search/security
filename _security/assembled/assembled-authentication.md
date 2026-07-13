---
api_key_in: []
api_specs:
- filename: assembled-people-api-openapi.yml
  format: yaml
  label: Assembled People API
  slug: assembled-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-people-api-openapi.yml
- filename: assembled-agent-state-api-openapi.yml
  format: yaml
  label: Assembled Agent State API
  slug: assembled-agent-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-agent-state-api-openapi.yml
- filename: assembled-activities-api-openapi.yml
  format: yaml
  label: Assembled Activities API
  slug: assembled-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-activities-api-openapi.yml
- filename: assembled-filters-api-openapi.yml
  format: yaml
  label: Assembled Filters API
  slug: assembled-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-filters-api-openapi.yml
- filename: assembled-forecasts-api-openapi.yml
  format: yaml
  label: Assembled Forecasts API
  slug: assembled-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-forecasts-api-openapi.yml
- filename: assembled-time-off-api-openapi.yml
  format: yaml
  label: Assembled Time Off API
  slug: assembled-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-time-off-api-openapi.yml
- filename: assembled-requirements-api-openapi.yml
  format: yaml
  label: Assembled Requirements API
  slug: assembled-requirements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-requirements-api-openapi.yml
- filename: assembled-scheduling-rules-api-openapi.yml
  format: yaml
  label: Assembled Scheduling Rules API
  slug: assembled-scheduling-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-scheduling-rules-api-openapi.yml
- filename: assembled-conversations-api-openapi.yml
  format: yaml
  label: Assembled Conversations API
  slug: assembled-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-conversations-api-openapi.yml
- filename: assembled-reports-api-openapi.yml
  format: yaml
  label: Assembled Reports API
  slug: assembled-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-reports-api-openapi.yml
- filename: assembled-qa-api-openapi.yml
  format: yaml
  label: Assembled QA API
  slug: assembled-qa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-qa-api-openapi.yml
- filename: assembled-assist-api-openapi.yml
  format: yaml
  label: Assembled Assist API
  slug: assembled-assist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-assist-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Assembled Authentication
name_suffix: Authentication
oauth_flows: []
overview: Assembled secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Assembled
provider_slug: assembled
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/assembled-activities-api-openapi.yml
  - openapi/assembled-agent-state-api-openapi.yml
  - openapi/assembled-assist-api-openapi.yml
  - openapi/assembled-conversations-api-openapi.yml
  - openapi/assembled-filters-api-openapi.yml
  - openapi/assembled-forecasts-api-openapi.yml
  - openapi/assembled-people-api-openapi.yml
  - openapi/assembled-qa-api-openapi.yml
  - openapi/assembled-reports-api-openapi.yml
  - openapi/assembled-requirements-api-openapi.yml
  - openapi/assembled-scheduling-rules-api-openapi.yml
  - openapi/assembled-time-off-api-openapi.yml
  type: http
slug: assembled-authentication
source_filename: assembled-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/assembled-activities-api-openapi.yml, openapi/assembled-agent-state-api-openapi.yml,\n  openapi/assembled-assist-api-openapi.yml, openapi/assembled-conversations-api-openapi.yml,\n  openapi/assembled-filters-api-openapi.yml, openapi/assembled-forecasts-api-openapi.yml, openapi/assembled-people-api-openapi.yml,\n  openapi/assembled-qa-api-openapi.yml, openapi/assembled-reports-api-openapi.yml, openapi/assembled-requirements-api-openapi.yml,\n  openapi/assembled-scheduling-rules-api-openapi.yml, openapi/assembled-time-off-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/assembled-activities-api-openapi.yml\n  - openapi/assembled-agent-state-api-openapi.yml\n  - openapi/assembled-assist-api-openapi.yml\n  - openapi/assembled-conversations-api-openapi.yml\n  - openapi/assembled-filters-api-openapi.yml\n  - openapi/assembled-forecasts-api-openapi.yml\n\
  \  - openapi/assembled-people-api-openapi.yml\n  - openapi/assembled-qa-api-openapi.yml\n  - openapi/assembled-reports-api-openapi.yml\n  - openapi/assembled-requirements-api-openapi.yml\n  - openapi/assembled-scheduling-rules-api-openapi.yml\n  - openapi/assembled-time-off-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/authentication/assembled-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Support
- Workforce Management
- WFM
- AI Agents
- AI Copilot
- Contact Center
- Customer Experience
- Support Operations
- Scheduling
- Forecasting
- Quality Assurance
- Vendor Management
- BPO
---
