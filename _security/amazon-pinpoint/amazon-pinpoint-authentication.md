---
api_key_in:
- header
api_specs:
- filename: amazon-pinpoint-openapi.yml
  format: yaml
  label: Amazon Pinpoint API
  slug: amazon-pinpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/openapi/amazon-pinpoint-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Pinpoint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Pinpoint secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-pinpoint-openapi-original.yaml
  - openapi/amazon-pinpoint-openapi.yml
  type: apiKey
slug: amazon-pinpoint-authentication
source_filename: amazon-pinpoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-pinpoint-openapi-original.yaml, openapi/amazon-pinpoint-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-pinpoint-openapi-original.yaml\n  - openapi/amazon-pinpoint-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/authentication/amazon-pinpoint-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
---
