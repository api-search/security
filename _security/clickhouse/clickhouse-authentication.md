---
api_key_in:
- header
api_specs:
- filename: clickhouse-clickhouse-http-interface-api-openapi.yml
  format: yaml
  label: ClickHouse ClickHouse HTTP Interface API
  slug: clickhouse-clickhouse-http-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/openapi/clickhouse-clickhouse-http-interface-api-openapi.yml
- filename: clickhouse-ping-api-openapi.yml
  format: yaml
  label: ClickHouse Ping API
  slug: clickhouse-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/openapi/clickhouse-ping-api-openapi.yml
- filename: clickhouse-play-api-openapi.yml
  format: yaml
  label: ClickHouse Play API
  slug: clickhouse-play-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/openapi/clickhouse-play-api-openapi.yml
- filename: clickhouse-replicas-status-api-openapi.yml
  format: yaml
  label: ClickHouse Replicas Status API
  slug: clickhouse-replicas-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/openapi/clickhouse-replicas-status-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Clickhouse Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClickHouse secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ClickHouse
provider_slug: clickhouse
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/clickhouse-openapi.yml
  type: http
- in: header
  name: clickhouseHeaders
  parameter: X-ClickHouse-User
  sources:
  - openapi/clickhouse-openapi.yml
  type: apiKey
slug: clickhouse-authentication
source_filename: clickhouse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/clickhouse-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/clickhouse-openapi.yml\n- name: clickhouseHeaders\n  type: apiKey\n  in: header\n  parameter: X-ClickHouse-User\n  sources:\n  - openapi/clickhouse-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickhouse/refs/heads/main/authentication/clickhouse-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Analytics
- Cloud Database
- Column-Oriented
- Database
- OLAP
- Open Source
- Real-Time
- SQL
---
