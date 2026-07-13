---
api_key_in:
- header
api_specs:
- filename: allquiet-openapi.yml
  format: yaml
  label: All Quiet Incidents API
  slug: incidents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allquiet/refs/heads/main/openapi/allquiet-openapi.yml
- filename: allquiet-openapi.yml
  format: yaml
  label: All Quiet Inbound Integrations API
  slug: inbound-integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allquiet/refs/heads/main/openapi/allquiet-openapi.yml
- filename: allquiet-openapi.yml
  format: yaml
  label: All Quiet Teams API
  slug: teams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allquiet/refs/heads/main/openapi/allquiet-openapi.yml
- filename: allquiet-openapi.yml
  format: yaml
  label: All Quiet On-Call Schedules API
  slug: on-call-schedules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allquiet/refs/heads/main/openapi/allquiet-openapi.yml
- filename: allquiet-openapi.yml
  format: yaml
  label: All Quiet Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allquiet/refs/heads/main/openapi/allquiet-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Allquiet Authentication
name_suffix: Authentication
oauth_flows: []
overview: All Quiet secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: All Quiet
provider_slug: allquiet
scheme_count: 2
schemes:
- description: Organization API key sent in the X-Api-Key header.
  in: header
  name: ApiKeyHeader
  parameter: X-Api-Key
  sources:
  - openapi/allquiet-openapi.yml
  type: apiKey
- description: Organization API key sent as a Bearer token in the Authorization header.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/allquiet-openapi.yml
  type: http
slug: allquiet-authentication
source_filename: allquiet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/allquiet-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Organization API key sent in the X-Api-Key header.\n  sources:\n  - openapi/allquiet-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Organization API key sent as a Bearer token in the Authorization header.\n  sources:\n  - openapi/allquiet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allquiet/refs/heads/main/authentication/allquiet-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Incident Management
- On-Call
- Alerting
- Incident Response
- DevOps
---
