---
api_key_in:
- header
api_specs:
- filename: firehydrant-api-openapi.yml
  format: yaml
  label: FireHydrant
  slug: firehydrant
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-api-openapi.yml
- filename: firehydrant-audits-api-openapi.yml
  format: yaml
  label: FireHydrant Audits API
  slug: firehydrant-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-audits-api-openapi.yml
- filename: firehydrant-change-events-api-openapi.yml
  format: yaml
  label: FireHydrant Change Events API
  slug: firehydrant-change-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-change-events-api-openapi.yml
- filename: firehydrant-changes-api-openapi.yml
  format: yaml
  label: FireHydrant Changes API
  slug: firehydrant-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-changes-api-openapi.yml
- filename: firehydrant-conversations-api-openapi.yml
  format: yaml
  label: FireHydrant Conversations API
  slug: firehydrant-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-conversations-api-openapi.yml
- filename: firehydrant-environments-api-openapi.yml
  format: yaml
  label: FireHydrant Environments API
  slug: firehydrant-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-environments-api-openapi.yml
- filename: firehydrant-functionalities-api-openapi.yml
  format: yaml
  label: FireHydrant Functionalities API
  slug: firehydrant-functionalities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-functionalities-api-openapi.yml
- filename: firehydrant-incidents-api-openapi.yml
  format: yaml
  label: FireHydrant Incidents API
  slug: firehydrant-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-incidents-api-openapi.yml
- filename: firehydrant-ping-api-openapi.yml
  format: yaml
  label: FireHydrant Ping API
  slug: firehydrant-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-ping-api-openapi.yml
- filename: firehydrant-priorities-api-openapi.yml
  format: yaml
  label: FireHydrant Priorities API
  slug: firehydrant-priorities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-priorities-api-openapi.yml
- filename: firehydrant-runbooks-api-openapi.yml
  format: yaml
  label: FireHydrant Runbooks API
  slug: firehydrant-runbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-runbooks-api-openapi.yml
- filename: firehydrant-scheduled-maintenances-api-openapi.yml
  format: yaml
  label: FireHydrant Scheduled Maintenances API
  slug: firehydrant-scheduled-maintenances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-scheduled-maintenances-api-openapi.yml
- filename: firehydrant-services-api-openapi.yml
  format: yaml
  label: FireHydrant Services API
  slug: firehydrant-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-services-api-openapi.yml
- filename: firehydrant-severities-api-openapi.yml
  format: yaml
  label: FireHydrant Severities API
  slug: firehydrant-severities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-severities-api-openapi.yml
- filename: firehydrant-signals-api-openapi.yml
  format: yaml
  label: FireHydrant Signals API
  slug: firehydrant-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-signals-api-openapi.yml
- filename: firehydrant-teams-api-openapi.yml
  format: yaml
  label: FireHydrant Teams API
  slug: firehydrant-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/openapi/firehydrant-teams-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Firehydrant Authentication
name_suffix: Authentication
oauth_flows: []
overview: FireHydrant secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: FireHydrant
provider_slug: firehydrant
scheme_count: 2
schemes:
- in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/firehydrant-api-openapi.yml
  type: apiKey
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/firehydrant-audits-api-openapi.yml
  - openapi/firehydrant-change-events-api-openapi.yml
  - openapi/firehydrant-changes-api-openapi.yml
  - openapi/firehydrant-conversations-api-openapi.yml
  - openapi/firehydrant-environments-api-openapi.yml
  - openapi/firehydrant-functionalities-api-openapi.yml
  - openapi/firehydrant-incidents-api-openapi.yml
  - openapi/firehydrant-ping-api-openapi.yml
  - openapi/firehydrant-priorities-api-openapi.yml
  - openapi/firehydrant-runbooks-api-openapi.yml
  - openapi/firehydrant-scheduled-maintenances-api-openapi.yml
  - openapi/firehydrant-services-api-openapi.yml
  - openapi/firehydrant-severities-api-openapi.yml
  - openapi/firehydrant-signals-api-openapi.yml
  - openapi/firehydrant-teams-api-openapi.yml
  type: http
slug: firehydrant-authentication
source_filename: firehydrant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: derived\nsource: openapi/firehydrant-api-openapi.yml, openapi/firehydrant-audits-api-openapi.yml, openapi/firehydrant-change-events-api-openapi.yml,\n  openapi/firehydrant-changes-api-openapi.yml, openapi/firehydrant-conversations-api-openapi.yml,\n  openapi/firehydrant-environments-api-openapi.yml, openapi/firehydrant-functionalities-api-openapi.yml,\n  openapi/firehydrant-incidents-api-openapi.yml, openapi/firehydrant-ping-api-openapi.yml, openapi/firehydrant-priorities-api-openapi.yml,\n  openapi/firehydrant-runbooks-api-openapi.yml, openapi/firehydrant-scheduled-maintenances-api-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/firehydrant-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/firehydrant-audits-api-openapi.yml\n  - openapi/firehydrant-change-events-api-openapi.yml\n\
  \  - openapi/firehydrant-changes-api-openapi.yml\n  - openapi/firehydrant-conversations-api-openapi.yml\n  - openapi/firehydrant-environments-api-openapi.yml\n  - openapi/firehydrant-functionalities-api-openapi.yml\n  - openapi/firehydrant-incidents-api-openapi.yml\n  - openapi/firehydrant-ping-api-openapi.yml\n  - openapi/firehydrant-priorities-api-openapi.yml\n  - openapi/firehydrant-runbooks-api-openapi.yml\n  - openapi/firehydrant-scheduled-maintenances-api-openapi.yml\n  - openapi/firehydrant-services-api-openapi.yml\n  - openapi/firehydrant-severities-api-openapi.yml\n  - openapi/firehydrant-signals-api-openapi.yml\n  - openapi/firehydrant-teams-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/authentication/firehydrant-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AIOps
- Incident Management
- On-Call
- Alerting
- Status Pages
- Runbooks
- Site Reliability Engineering
- Observability
- Retrospectives
- DevOps
---
