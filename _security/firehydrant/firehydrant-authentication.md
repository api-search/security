---
api_key_in: []
api_specs:
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
- http
description: ''
kind: authentication
layout: security
method: derived
name: Firehydrant Authentication
name_suffix: Authentication
oauth_flows: []
overview: FireHydrant secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FireHydrant
provider_slug: firehydrant
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/firehydrant-openapi.yml
  type: http
slug: firehydrant-authentication
source_filename: firehydrant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/firehydrant-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/firehydrant-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firehydrant/refs/heads/main/authentication/firehydrant-authentication.yml
summary_line: http · 1 scheme
tags:
- AIOps
- Incident Management
---
