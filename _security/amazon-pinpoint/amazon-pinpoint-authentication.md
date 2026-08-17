---
api_key_in:
- header
api_specs:
- filename: amazon-pinpoint-applications-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Applications API
  slug: amazon-pinpoint-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/openapi/amazon-pinpoint-applications-api-openapi.yml
- filename: amazon-pinpoint-apps-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Apps API
  slug: amazon-pinpoint-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/openapi/amazon-pinpoint-apps-api-openapi.yml
- filename: amazon-pinpoint-phone-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Phone API
  slug: amazon-pinpoint-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/openapi/amazon-pinpoint-phone-api-openapi.yml
- filename: amazon-pinpoint-recommenders-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Recommenders API
  slug: amazon-pinpoint-recommenders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/openapi/amazon-pinpoint-recommenders-api-openapi.yml
- filename: amazon-pinpoint-tags-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Tags API
  slug: amazon-pinpoint-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/openapi/amazon-pinpoint-tags-api-openapi.yml
- filename: amazon-pinpoint-templates-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Templates API
  slug: amazon-pinpoint-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/openapi/amazon-pinpoint-templates-api-openapi.yml
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
  - openapi/amazon-pinpoint-applications-api-openapi.yml
  - openapi/amazon-pinpoint-apps-api-openapi.yml
  - openapi/amazon-pinpoint-phone-api-openapi.yml
  - openapi/amazon-pinpoint-recommenders-api-openapi.yml
  - openapi/amazon-pinpoint-tags-api-openapi.yml
  - openapi/amazon-pinpoint-templates-api-openapi.yml
  type: apiKey
slug: amazon-pinpoint-authentication
source_filename: amazon-pinpoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/amazon-pinpoint-applications-api-openapi.yml, openapi/amazon-pinpoint-apps-api-openapi.yml,\n  openapi/amazon-pinpoint-phone-api-openapi.yml, openapi/amazon-pinpoint-recommenders-api-openapi.yml,\n  openapi/amazon-pinpoint-tags-api-openapi.yml, openapi/amazon-pinpoint-templates-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-pinpoint-applications-api-openapi.yml\n  - openapi/amazon-pinpoint-apps-api-openapi.yml\n  - openapi/amazon-pinpoint-phone-api-openapi.yml\n  - openapi/amazon-pinpoint-recommenders-api-openapi.yml\n  - openapi/amazon-pinpoint-tags-api-openapi.yml\n  - openapi/amazon-pinpoint-templates-api-openapi.yml\n"
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
