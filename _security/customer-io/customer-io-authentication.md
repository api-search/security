---
api_key_in: []
api_specs:
- filename: customer-io-track-api-openapi.yml
  format: yaml
  label: Customer.io Track API
  slug: track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customer-io/refs/heads/main/openapi/customer-io-track-api-openapi.yml
- filename: customer-io-app-api-openapi.yml
  format: yaml
  label: Customer.io App API
  slug: app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customer-io/refs/heads/main/openapi/customer-io-app-api-openapi.yml
- filename: customer-io-pipelines-api-openapi.yml
  format: yaml
  label: Customer.io Pipelines API
  slug: pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customer-io/refs/heads/main/openapi/customer-io-pipelines-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Customer Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Customer.io secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Customer.io
provider_slug: customer-io
scheme_count: 2
schemes:
- description: Bearer token authentication using your App API key. Pass the key in the Authorization header as Bearer {app_api_key}.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/customer-io-app-api-openapi.yml
  type: http
- description: Basic authentication using your CDP API key as the username with a blank password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/customer-io-pipelines-api-openapi.yml
  - openapi/customer-io-track-api-openapi.yml
  type: http
slug: customer-io-authentication
source_filename: customer-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/customer-io-app-api-openapi.yml, openapi/customer-io-pipelines-api-openapi.yml,\n  openapi/customer-io-track-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication using your App API key. Pass the key in the Authorization\n    header as Bearer {app_api_key}.\n  sources:\n  - openapi/customer-io-app-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication using your CDP API key as the username with a blank password.\n  sources:\n  - openapi/customer-io-pipelines-api-openapi.yml\n  - openapi/customer-io-track-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/customer-io/refs/heads/main/authentication/customer-io-authentication.yml
summary_line: http · 2 schemes
tags:
- Behavioral Data
- Broadcasts
- Campaigns
- CDP
- Customer Data
- Customer Data Platform
- Data Ingestion
- Email
- Event Tracking
- Marketing Automation
- Messaging
- Push Notifications
- Segments
- SMS
- Transactional Email
---
