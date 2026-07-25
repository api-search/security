---
api_key_in:
- header
api_specs:
- filename: adobe-analytics-livestream-asyncapi.yml
  format: yaml
  label: Adobe Analytics Livestream API
  slug: adobe-analytics-livestream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/asyncapi/adobe-analytics-livestream-asyncapi.yml
- filename: adobe-analytics-annotations-api-openapi.yml
  format: yaml
  label: Adobe Analytics Annotations API
  slug: adobe-analytics-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-annotations-api-openapi.yml
- filename: adobe-analytics-calculated-metrics-api-openapi.yml
  format: yaml
  label: Adobe Analytics Calculated Metrics API
  slug: adobe-analytics-calculated-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-calculated-metrics-api-openapi.yml
- filename: adobe-analytics-date-ranges-api-openapi.yml
  format: yaml
  label: Adobe Analytics Date Ranges API
  slug: adobe-analytics-date-ranges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-date-ranges-api-openapi.yml
- filename: adobe-analytics-dimensions-api-openapi.yml
  format: yaml
  label: Adobe Analytics Dimensions API
  slug: adobe-analytics-dimensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-dimensions-api-openapi.yml
- filename: adobe-analytics-events-api-openapi.yml
  format: yaml
  label: Adobe Analytics Events API
  slug: adobe-analytics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-events-api-openapi.yml
- filename: adobe-analytics-jobs-api-openapi.yml
  format: yaml
  label: Adobe Analytics Jobs API
  slug: adobe-analytics-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-jobs-api-openapi.yml
- filename: adobe-analytics-metrics-api-openapi.yml
  format: yaml
  label: Adobe Analytics Metrics API
  slug: adobe-analytics-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-metrics-api-openapi.yml
- filename: adobe-analytics-report-suites-api-openapi.yml
  format: yaml
  label: Adobe Analytics Report Suites API
  slug: adobe-analytics-report-suites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-report-suites-api-openapi.yml
- filename: adobe-analytics-reports-api-openapi.yml
  format: yaml
  label: Adobe Analytics Reports API
  slug: adobe-analytics-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-reports-api-openapi.yml
- filename: adobe-analytics-segments-api-openapi.yml
  format: yaml
  label: Adobe Analytics Segments API
  slug: adobe-analytics-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-segments-api-openapi.yml
- filename: adobe-analytics-server-call-estimate-api-openapi.yml
  format: yaml
  label: Adobe Analytics Server Call Estimate API
  slug: adobe-analytics-server-call-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/openapi/adobe-analytics-server-call-estimate-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Adobe Analytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adobe Analytics secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Adobe Analytics
provider_slug: adobe-analytics
scheme_count: 2
schemes:
- description: OAuth 2.0 access token from Adobe IMS
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/adobe-analytics-api-openapi.yml
  - openapi/adobe-analytics-bulk-data-insertion-api-openapi.yml
  - openapi/adobe-analytics-data-repair-api-openapi.yml
  type: http
- description: Adobe Developer Console API key
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/adobe-analytics-api-openapi.yml
  - openapi/adobe-analytics-bulk-data-insertion-api-openapi.yml
  - openapi/adobe-analytics-data-repair-api-openapi.yml
  type: apiKey
slug: adobe-analytics-authentication
source_filename: adobe-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-analytics-api-openapi.yml, openapi/adobe-analytics-bulk-data-insertion-api-openapi.yml,\n  openapi/adobe-analytics-data-repair-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token from Adobe IMS\n  sources:\n  - openapi/adobe-analytics-api-openapi.yml\n  - openapi/adobe-analytics-bulk-data-insertion-api-openapi.yml\n  - openapi/adobe-analytics-data-repair-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Adobe Developer Console API key\n  sources:\n  - openapi/adobe-analytics-api-openapi.yml\n  - openapi/adobe-analytics-bulk-data-insertion-api-openapi.yml\n  - openapi/adobe-analytics-data-repair-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/authentication/adobe-analytics-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
---
