---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-pinpoint-apps-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Apps API
  slug: amazon-pinpoint-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-apps-api-openapi.yml
- filename: amazon-pinpoint-phone-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Phone API
  slug: amazon-pinpoint-phone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-phone-api-openapi.yml
- filename: amazon-pinpoint-recommenders-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Recommenders API
  slug: amazon-pinpoint-recommenders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-recommenders-api-openapi.yml
- filename: amazon-pinpoint-tags-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Tags API
  slug: amazon-pinpoint-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-tags-api-openapi.yml
- filename: amazon-pinpoint-templates-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Templates API
  slug: amazon-pinpoint-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-templates-api-openapi.yml
- filename: amazon-pinpoint-campaigns-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Campaigns API
  slug: amazon-pinpoint-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-campaigns-api-openapi.yml
- filename: amazon-pinpoint-channels-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Channels API
  slug: amazon-pinpoint-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-channels-api-openapi.yml
- filename: amazon-pinpoint-email-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Email API
  slug: amazon-pinpoint-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-email-api-openapi.yml
- filename: amazon-pinpoint-endpoints-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Endpoints API
  slug: amazon-pinpoint-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-endpoints-api-openapi.yml
- filename: amazon-pinpoint-eventstream-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Eventstream API
  slug: amazon-pinpoint-eventstream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-eventstream-api-openapi.yml
- filename: amazon-pinpoint-execution-metrics-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Execution Metrics API
  slug: amazon-pinpoint-execution-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-execution-metrics-api-openapi.yml
- filename: amazon-pinpoint-inapp-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Inapp API
  slug: amazon-pinpoint-inapp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-inapp-api-openapi.yml
- filename: amazon-pinpoint-jobs-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Jobs API
  slug: amazon-pinpoint-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-jobs-api-openapi.yml
- filename: amazon-pinpoint-journeys-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Journeys API
  slug: amazon-pinpoint-journeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-journeys-api-openapi.yml
- filename: amazon-pinpoint-kpis-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Kpis API
  slug: amazon-pinpoint-kpis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-kpis-api-openapi.yml
- filename: amazon-pinpoint-operations-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Operations API
  slug: amazon-pinpoint-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-operations-api-openapi.yml
- filename: amazon-pinpoint-push-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Push API
  slug: amazon-pinpoint-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-push-api-openapi.yml
- filename: amazon-pinpoint-segments-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Segments API
  slug: amazon-pinpoint-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-segments-api-openapi.yml
- filename: amazon-pinpoint-sms-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Sms API
  slug: amazon-pinpoint-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-sms-api-openapi.yml
- filename: amazon-pinpoint-versions-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Versions API
  slug: amazon-pinpoint-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-versions-api-openapi.yml
- filename: amazon-pinpoint-voice-api-openapi.yml
  format: yaml
  label: Amazon Pinpoint Pinpoint Voice API
  slug: amazon-pinpoint-voice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-pinpoint/openapi/amazon-pinpoint-voice-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/amazon-pinpoint/authentication/amazon-pinpoint-authentication.yml
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
