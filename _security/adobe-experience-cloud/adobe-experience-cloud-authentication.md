---
api_key_in:
- header
api_specs:
- filename: adobe-analytics-api-openapi.yml
  format: yaml
  label: Adobe Analytics 2.0 API
  slug: analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/openapi/adobe-analytics-api-openapi.yml
- filename: adobe-experience-platform-api-openapi.yml
  format: yaml
  label: Adobe Experience Platform API
  slug: experience-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/openapi/adobe-experience-platform-api-openapi.yml
- filename: adobe-target-api-openapi.yml
  format: yaml
  label: Adobe Target API
  slug: target-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/openapi/adobe-target-api-openapi.yml
- filename: adobe-journey-optimizer-api-openapi.yml
  format: yaml
  label: Adobe Journey Optimizer API
  slug: journey-optimizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/openapi/adobe-journey-optimizer-api-openapi.yml
- filename: adobe-campaign-api-openapi.yml
  format: yaml
  label: Adobe Campaign API
  slug: campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/openapi/adobe-campaign-api-openapi.yml
- filename: adobe-io-events-asyncapi.yml
  format: yaml
  label: Adobe I/O Events
  slug: io-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/asyncapi/adobe-io-events-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Adobe Experience Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adobe Experience Cloud secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained via Adobe I/O.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/adobe-analytics-api-openapi.yml
  - openapi/adobe-campaign-api-openapi.yml
  - openapi/adobe-experience-platform-api-openapi.yml
  - openapi/adobe-journey-optimizer-api-openapi.yml
  - openapi/adobe-target-api-openapi.yml
  type: http
- description: Adobe I/O client API key.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/adobe-analytics-api-openapi.yml
  - openapi/adobe-campaign-api-openapi.yml
  - openapi/adobe-experience-platform-api-openapi.yml
  - openapi/adobe-journey-optimizer-api-openapi.yml
  - openapi/adobe-target-api-openapi.yml
  type: apiKey
slug: adobe-experience-cloud-authentication
source_filename: adobe-experience-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-analytics-api-openapi.yml, openapi/adobe-campaign-api-openapi.yml, openapi/adobe-experience-platform-api-openapi.yml,\n  openapi/adobe-journey-optimizer-api-openapi.yml, openapi/adobe-target-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained via Adobe I/O.\n  sources:\n  - openapi/adobe-analytics-api-openapi.yml\n  - openapi/adobe-campaign-api-openapi.yml\n  - openapi/adobe-experience-platform-api-openapi.yml\n  - openapi/adobe-journey-optimizer-api-openapi.yml\n  - openapi/adobe-target-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Adobe I/O client API key.\n  sources:\n  - openapi/adobe-analytics-api-openapi.yml\n  - openapi/adobe-campaign-api-openapi.yml\n  - openapi/adobe-experience-platform-api-openapi.yml\n\
  \  - openapi/adobe-journey-optimizer-api-openapi.yml\n  - openapi/adobe-target-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/authentication/adobe-experience-cloud-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
---
