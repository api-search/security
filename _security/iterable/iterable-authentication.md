---
api_key_in:
- header
api_specs:
- filename: iterable-export-api-openapi.yml
  format: yaml
  label: Iterable Export API
  slug: export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-export-api-openapi.yml
- filename: iterable-campaigns-api-openapi.yml
  format: yaml
  label: Iterable Campaigns API
  slug: iterable-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-campaigns-api-openapi.yml
- filename: iterable-catalogs-api-openapi.yml
  format: yaml
  label: Iterable Catalogs API
  slug: iterable-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-catalogs-api-openapi.yml
- filename: iterable-channels-api-openapi.yml
  format: yaml
  label: Iterable Channels API
  slug: iterable-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-channels-api-openapi.yml
- filename: iterable-commerce-api-openapi.yml
  format: yaml
  label: Iterable Commerce API
  slug: iterable-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-commerce-api-openapi.yml
- filename: iterable-email-api-openapi.yml
  format: yaml
  label: Iterable Email API
  slug: iterable-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-email-api-openapi.yml
- filename: iterable-events-api-openapi.yml
  format: yaml
  label: Iterable Events API
  slug: iterable-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-events-api-openapi.yml
- filename: iterable-experimentmetrics-api-openapi.yml
  format: yaml
  label: Iterable ExperimentMetrics API
  slug: iterable-experimentmetrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-experimentmetrics-api-openapi.yml
- filename: iterable-experiments-api-openapi.yml
  format: yaml
  label: Iterable Experiments API
  slug: iterable-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-experiments-api-openapi.yml
- filename: iterable-inapp-api-openapi.yml
  format: yaml
  label: Iterable InApp API
  slug: iterable-inapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-inapp-api-openapi.yml
- filename: iterable-lists-api-openapi.yml
  format: yaml
  label: Iterable Lists API
  slug: iterable-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-lists-api-openapi.yml
- filename: iterable-messagetypes-api-openapi.yml
  format: yaml
  label: Iterable MessageTypes API
  slug: iterable-messagetypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-messagetypes-api-openapi.yml
- filename: iterable-metadata-api-openapi.yml
  format: yaml
  label: Iterable Metadata API
  slug: iterable-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-metadata-api-openapi.yml
- filename: iterable-push-api-openapi.yml
  format: yaml
  label: Iterable Push API
  slug: iterable-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-push-api-openapi.yml
- filename: iterable-sms-api-openapi.yml
  format: yaml
  label: Iterable SMS API
  slug: iterable-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-sms-api-openapi.yml
- filename: iterable-templates-api-openapi.yml
  format: yaml
  label: Iterable Templates API
  slug: iterable-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-templates-api-openapi.yml
- filename: iterable-users-api-openapi.yml
  format: yaml
  label: Iterable Users API
  slug: iterable-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-users-api-openapi.yml
- filename: iterable-webpush-api-openapi.yml
  format: yaml
  label: Iterable WebPush API
  slug: iterable-webpush-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-webpush-api-openapi.yml
- filename: iterable-workflows-api-openapi.yml
  format: yaml
  label: Iterable Workflows API
  slug: iterable-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-workflows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Iterable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Iterable secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Iterable
provider_slug: iterable
scheme_count: 1
schemes:
- description: Iterable API key passed in the Api-Key header. API keys can be created and managed in the Iterable project settings.
  in: header
  name: apiKeyAuth
  parameter: Api-Key
  sources:
  - openapi/iterable-export-api-openapi.yml
  - openapi/iterable-rest-api-openapi.yml
  type: apiKey
slug: iterable-authentication
source_filename: iterable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/iterable-export-api-openapi.yml, openapi/iterable-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: Iterable API key passed in the Api-Key header. API keys can be created and managed\n    in the Iterable project settings.\n  sources:\n  - openapi/iterable-export-api-openapi.yml\n  - openapi/iterable-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/authentication/iterable-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cross-Channel Messaging
- Customer Engagement
- Email
- Marketing Automation
- Push Notifications
- SMS
---
