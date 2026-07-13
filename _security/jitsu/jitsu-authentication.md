---
api_key_in:
- header
api_specs:
- filename: jitsu-openapi.yml
  format: yaml
  label: Jitsu Event Ingestion API (Track / Identify / Page)
  slug: event-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitsu/refs/heads/main/openapi/jitsu-openapi.yml
- filename: jitsu-openapi.yml
  format: yaml
  label: Jitsu Bulk / Batch API
  slug: bulk-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitsu/refs/heads/main/openapi/jitsu-openapi.yml
- filename: jitsu-openapi.yml
  format: yaml
  label: Jitsu Configuration / Management
  slug: configuration-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitsu/refs/heads/main/openapi/jitsu-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jitsu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jitsu secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Jitsu
provider_slug: jitsu
scheme_count: 2
schemes:
- description: Write Key in the form keyId:keySecret.
  in: header
  name: WriteKeyHeader
  parameter: X-Write-Key
  sources:
  - openapi/jitsu-openapi.yml
  type: apiKey
- description: HTTP Basic auth with the Write Key as the username (password empty).
  name: WriteKeyBasic
  scheme: basic
  sources:
  - openapi/jitsu-openapi.yml
  type: http
slug: jitsu-authentication
source_filename: jitsu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jitsu-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: WriteKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Write-Key\n  description: Write Key in the form keyId:keySecret.\n  sources:\n  - openapi/jitsu-openapi.yml\n- name: WriteKeyBasic\n  type: http\n  scheme: basic\n  description: HTTP Basic auth with the Write Key as the username (password empty).\n  sources:\n  - openapi/jitsu-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jitsu/refs/heads/main/authentication/jitsu-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Event Data
- CDP
- Data Pipeline
- Analytics
- Open Source
- Ingestion
---
