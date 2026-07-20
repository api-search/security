---
api_key_in:
- header
- query
api_specs:
- filename: apptentive-openapi-original.yml
  format: yaml
  label: Apptentive Data API
  slug: apptentive-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apptentive/refs/heads/main/openapi/apptentive-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Apptentive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apptentive secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apptentive
provider_slug: apptentive
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  query_alt: api_key
  sources:
  - openapi/apptentive-openapi-original.yml
  type: apiKey
slug: apptentive-authentication
source_filename: apptentive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/apptentive-openapi-original.yml\ndocs: https://help.alchemer.com/help/alchemer-digital-api\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nnotes: >-\n  API keys are generated and scoped by the customer from the Alchemer Digital dashboard\n  (\"completely self-manage API key generation and scope\"). Pass as the X-API-KEY header,\n  or optionally as the api_key query parameter. All access is over HTTPS/TLS.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  query_alt: api_key\n  sources:\n  - openapi/apptentive-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apptentive/refs/heads/main/authentication/apptentive-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Enterprise
- Mobile
- Customer Feedback
- Surveys
- Analytics
- Customer Engagement
- Voice of Customer
---
