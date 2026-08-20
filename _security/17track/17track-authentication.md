---
api_key_in:
- header
api_specs:
- filename: 17track-tracking-api-openapi.yml
  format: yaml
  label: 17TRACK Tracking API
  slug: 17track-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/17track/refs/heads/main/openapi/17track-tracking-api-openapi.yml
- filename: 17track-webhooks-api-openapi.yml
  format: yaml
  label: 17TRACK Webhooks API
  slug: 17track-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/17track/refs/heads/main/openapi/17track-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: 17Track Authentication
name_suffix: Authentication
oauth_flows: []
overview: 17TRACK secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 17TRACK
provider_slug: 17track
scheme_count: 1
schemes:
- description: API access key obtained from Management Console > Settings > Security > Access Key. Key updates take effect within 5 minutes.
  in: header
  name: ApiKeyAuth
  parameter: 17token
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: 17track-authentication
source_filename: 17track-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: 17token\n  description: API access key obtained from Management Console > Settings > Security > Access\n    Key. Key updates take effect within 5 minutes.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/17track/refs/heads/main/authentication/17track-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Shipping
- Package Tracking
- Logistics
- Carriers
- Delivery
- Webhook
---
