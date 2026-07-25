---
api_key_in:
- header
api_specs:
- filename: overops-alerts-api-openapi.yml
  format: yaml
  label: Overops Alerts API
  slug: overops-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-alerts-api-openapi.yml
- filename: overops-categories-api-openapi.yml
  format: yaml
  label: Overops Categories API
  slug: overops-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-categories-api-openapi.yml
- filename: overops-code-redaction-api-openapi.yml
  format: yaml
  label: Overops Code Redaction API
  slug: overops-code-redaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-code-redaction-api-openapi.yml
- filename: overops-data-redaction-api-openapi.yml
  format: yaml
  label: Overops Data Redaction API
  slug: overops-data-redaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-data-redaction-api-openapi.yml
- filename: overops-entry-points-api-openapi.yml
  format: yaml
  label: Overops Entry Points API
  slug: overops-entry-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-entry-points-api-openapi.yml
- filename: overops-environment-management-api-openapi.yml
  format: yaml
  label: Overops Environment Management API
  slug: overops-environment-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-environment-management-api-openapi.yml
- filename: overops-events-api-openapi.yml
  format: yaml
  label: Overops Events API
  slug: overops-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-events-api-openapi.yml
- filename: overops-general-api-openapi.yml
  format: yaml
  label: Overops General API
  slug: overops-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-general-api-openapi.yml
- filename: overops-labels-api-openapi.yml
  format: yaml
  label: Overops Labels API
  slug: overops-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-labels-api-openapi.yml
- filename: overops-publish-metrics-api-openapi.yml
  format: yaml
  label: Overops Publish Metrics API
  slug: overops-publish-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-publish-metrics-api-openapi.yml
- filename: overops-system-metrics-api-openapi.yml
  format: yaml
  label: Overops System Metrics API
  slug: overops-system-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-system-metrics-api-openapi.yml
- filename: overops-team-management-api-openapi.yml
  format: yaml
  label: Overops Team Management API
  slug: overops-team-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-team-management-api-openapi.yml
- filename: overops-timers-api-openapi.yml
  format: yaml
  label: Overops Timers API
  slug: overops-timers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-timers-api-openapi.yml
- filename: overops-udfs-api-openapi.yml
  format: yaml
  label: Overops UDFs API
  slug: overops-udfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-udfs-api-openapi.yml
- filename: overops-view-metrics-api-openapi.yml
  format: yaml
  label: Overops View Metrics API
  slug: overops-view-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-view-metrics-api-openapi.yml
- filename: overops-views-api-openapi.yml
  format: yaml
  label: Overops Views API
  slug: overops-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/openapi/overops-views-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Overops Authentication
name_suffix: Authentication
oauth_flows: []
overview: Overops secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Overops
provider_slug: overops
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/overops-openapi-original.json
  type: http
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/overops-openapi-original.json
  type: apiKey
slug: overops-authentication
source_filename: overops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/overops-openapi-original.json\ndocs: https://doc.overops.com/reference\nnotes: >-\n  Confirmed against the OpenAPI info.description: authenticate with the X-API-KEY\n  header (generate under Settings -> Account Settings; recommended) or HTTP Basic\n  using a username:password combo.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/overops-openapi-original.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/overops-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overops/refs/heads/main/authentication/overops-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Observability
- Reliability
- Error Monitoring
- Application Performance
- Java
- DevOps
- Code Quality
---
