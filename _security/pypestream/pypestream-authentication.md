---
api_key_in:
- header
api_specs:
- filename: pypestream-reporting-api-openapi.json
  format: json
  label: Pypestream Reporting API
  slug: reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/openapi/pypestream-reporting-api-openapi.json
- filename: pypestream-contact-center-api-openapi.json
  format: json
  label: Pypestream Contact Center API
  slug: contact-center-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/openapi/pypestream-contact-center-api-openapi.json
- filename: pypestream-middleware-api-openapi.json
  format: json
  label: Pypestream Middleware API
  slug: middleware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/openapi/pypestream-middleware-api-openapi.json
- filename: pypestream-engagement-api-openapi.json
  format: json
  label: Pypestream Engagement API
  slug: engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/openapi/pypestream-engagement-api-openapi.json
- filename: pypestream-analytics-api-openapi.json
  format: json
  label: Pypestream Analytics API
  slug: analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/openapi/pypestream-analytics-api-openapi.json
- filename: pypestream-javascript-sdk-openapi.json
  format: json
  label: Pypestream JavaScript SDK API
  slug: javascript-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/openapi/pypestream-javascript-sdk-openapi.json
- filename: pypestream-insights-api-openapi.json
  format: json
  label: Pypestream Insights API
  slug: insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/openapi/pypestream-insights-api-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pypestream Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pypestream secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pypestream
provider_slug: pypestream
scheme_count: 4
schemes:
- name: APIKey
  scheme: bearer
  sources:
  - openapi/pypestream-analytics-api-openapi.json
  - openapi/pypestream-engagement-api-openapi.json
  type: http
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/pypestream-contact-center-api-openapi.json
  - openapi/pypestream-middleware-api-openapi.json
  - openapi/pypestream-reporting-api-openapi.json
  type: http
- in: header
  name: TokenHeader
  parameter: X-Pypestream-Token
  sources:
  - openapi/pypestream-contact-center-api-openapi.json
  - openapi/pypestream-middleware-api-openapi.json
  type: apiKey
- description: 'API key for accessing Pypestream services (if applicable).

    Note: The JavaScript SDK does not require API keys for client-side usage.'
  in: header
  name: ApiKey
  parameter: X-API-Key
  sources:
  - openapi/pypestream-javascript-sdk-openapi.json
  type: apiKey
slug: pypestream-authentication
source_filename: pypestream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/pypestream-analytics-api-openapi.json, openapi/pypestream-contact-center-api-openapi.json,\n  openapi/pypestream-engagement-api-openapi.json, openapi/pypestream-javascript-sdk-openapi.json,\n  openapi/pypestream-middleware-api-openapi.json, openapi/pypestream-reporting-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: APIKey\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/pypestream-analytics-api-openapi.json\n  - openapi/pypestream-engagement-api-openapi.json\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/pypestream-contact-center-api-openapi.json\n  - openapi/pypestream-middleware-api-openapi.json\n  - openapi/pypestream-reporting-api-openapi.json\n- name: TokenHeader\n  type: apiKey\n  in: header\n  parameter: X-Pypestream-Token\n  sources:\n  - openapi/pypestream-contact-center-api-openapi.json\n  - openapi/pypestream-middleware-api-openapi.json\n\
  - name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: |-\n    API key for accessing Pypestream services (if applicable).\n    Note: The JavaScript SDK does not require API keys for client-side usage.\n  sources:\n  - openapi/pypestream-javascript-sdk-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pypestream/refs/heads/main/authentication/pypestream-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Conversational AI
- Agentic AI
- Contact Center
- Customer Service
- Customer Engagement
- Chatbots
- Voice AI
- Messaging
- Analytics
- Enterprise Software
---
