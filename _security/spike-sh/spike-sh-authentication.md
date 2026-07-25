---
api_key_in:
- header
api_specs:
- filename: spike-sh-alert-rules-api-openapi.yml
  format: yaml
  label: Spike.sh Alert Rules API
  slug: spike-sh-alert-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-alert-rules-api-openapi.yml
- filename: spike-sh-components-api-openapi.yml
  format: yaml
  label: Spike.sh Components API
  slug: spike-sh-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-components-api-openapi.yml
- filename: spike-sh-escalations-api-openapi.yml
  format: yaml
  label: Spike.sh Escalations API
  slug: spike-sh-escalations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-escalations-api-openapi.yml
- filename: spike-sh-incident-actions-api-openapi.yml
  format: yaml
  label: Spike.sh Incident Actions API
  slug: spike-sh-incident-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-incident-actions-api-openapi.yml
- filename: spike-sh-incidents-api-openapi.yml
  format: yaml
  label: Spike.sh Incidents API
  slug: spike-sh-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-incidents-api-openapi.yml
- filename: spike-sh-integrations-api-openapi.yml
  format: yaml
  label: Spike.sh Integrations API
  slug: spike-sh-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-integrations-api-openapi.yml
- filename: spike-sh-on-call-overrides-api-openapi.yml
  format: yaml
  label: Spike.sh On-Call Overrides API
  slug: spike-sh-on-call-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-on-call-overrides-api-openapi.yml
- filename: spike-sh-on-call-schedules-api-openapi.yml
  format: yaml
  label: Spike.sh On-Call Schedules API
  slug: spike-sh-on-call-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-on-call-schedules-api-openapi.yml
- filename: spike-sh-orgs-api-openapi.yml
  format: yaml
  label: Spike.sh Orgs API
  slug: spike-sh-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-orgs-api-openapi.yml
- filename: spike-sh-planned-maintenances-api-openapi.yml
  format: yaml
  label: Spike.sh Planned Maintenances API
  slug: spike-sh-planned-maintenances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-planned-maintenances-api-openapi.yml
- filename: spike-sh-services-api-openapi.yml
  format: yaml
  label: Spike.sh Services API
  slug: spike-sh-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-services-api-openapi.yml
- filename: spike-sh-status-page-incidents-api-openapi.yml
  format: yaml
  label: Spike.sh Status Page Incidents API
  slug: spike-sh-status-page-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-status-page-incidents-api-openapi.yml
- filename: spike-sh-status-pages-api-openapi.yml
  format: yaml
  label: Spike.sh Status Pages API
  slug: spike-sh-status-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-status-pages-api-openapi.yml
- filename: spike-sh-subscribers-api-openapi.yml
  format: yaml
  label: Spike.sh Subscribers API
  slug: spike-sh-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-subscribers-api-openapi.yml
- filename: spike-sh-suppressed-incidents-api-openapi.yml
  format: yaml
  label: Spike.sh Suppressed Incidents API
  slug: spike-sh-suppressed-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-suppressed-incidents-api-openapi.yml
- filename: spike-sh-teams-api-openapi.yml
  format: yaml
  label: Spike.sh Teams API
  slug: spike-sh-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-teams-api-openapi.yml
- filename: spike-sh-users-api-openapi.yml
  format: yaml
  label: Spike.sh Users API
  slug: spike-sh-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/openapi/spike-sh-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spike Sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spike.sh secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spike.sh
provider_slug: spike-sh
scheme_count: 1
schemes:
- description: API key generated from https://app.spike.sh/api
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/spike-sh-openapi.yml
  type: apiKey
slug: spike-sh-authentication
source_filename: spike-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spike-sh-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key generated from https://app.spike.sh/api\n  sources:\n  - openapi/spike-sh-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/authentication/spike-sh-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Incident Management
- On-Call
- Alerting
- Escalation Policies
- Status Pages
- Monitoring
- DevOps
- SRE
---
