---
api_key_in:
- header
api_specs:
- filename: loconav-integration-openapi.yml
  format: yaml
  label: LocoNav Integration API
  slug: loconav-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/openapi/loconav-integration-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Loconav Authentication
name_suffix: Authentication
oauth_flows: []
overview: LocoNav secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LocoNav
provider_slug: loconav
scheme_count: 1
schemes:
- description: User-level API token supplied in the User-Authentication request header. Each user is assigned a unique auth token, provisioned by a LocoNav SPOC (single point of contact). Incorrect or missing credentials return 401 Unauthorized.
  in: header
  name: UserAuthentication
  parameter: User-Authentication
  sources:
  - openapi/loconav-integration-openapi.yml
  token_provisioning: LocoNav SPOC (manual, per user)
  type: apiKey
slug: loconav-authentication
source_filename: loconav-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/loconav-integration-openapi.yml\ndocs: https://developers.loconav.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: UserAuthentication\n  type: apiKey\n  in: header\n  parameter: User-Authentication\n  description: >-\n    User-level API token supplied in the User-Authentication request header.\n    Each user is assigned a unique auth token, provisioned by a LocoNav SPOC\n    (single point of contact). Incorrect or missing credentials return 401\n    Unauthorized.\n  token_provisioning: LocoNav SPOC (manual, per user)\n  sources:\n  - openapi/loconav-integration-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loconav/refs/heads/main/authentication/loconav-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fleet Management
- Telematics
- GPS Tracking
- Vehicle Tracking
- Transportation
- Logistics
- IoT
- Video Telematics
- Webhooks
---
