---
api_key_in:
- header
api_specs:
- filename: myscale-openapi.yml
  format: yaml
  label: MyScale SQL Interface (ClickHouse HTTP)
  slug: myscale-sql-http-interface
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myscale/refs/heads/main/openapi/myscale-openapi.yml
- filename: myscale-openapi.yml
  format: yaml
  label: MyScale Vector Search (SQL)
  slug: myscale-vector-search-sql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myscale/refs/heads/main/openapi/myscale-openapi.yml
- filename: myscale-openapi.yml
  format: yaml
  label: MyScale Python SDK (clickhouse-connect)
  slug: myscale-python-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/myscale/refs/heads/main/openapi/myscale-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Myscale Authentication
name_suffix: Authentication
oauth_flows: []
overview: MyScale secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MyScale
provider_slug: myscale
scheme_count: 3
schemes:
- description: Cluster username and password (from the MyScale Cloud console Connection Details) supplied as HTTP Basic credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/myscale-openapi.yml
  type: http
- description: Cluster username, paired with X-ClickHouse-Key.
  in: header
  name: clickhouseUserHeader
  parameter: X-ClickHouse-User
  sources:
  - openapi/myscale-openapi.yml
  type: apiKey
- description: Cluster password, paired with X-ClickHouse-User.
  in: header
  name: clickhouseKeyHeader
  parameter: X-ClickHouse-Key
  sources:
  - openapi/myscale-openapi.yml
  type: apiKey
slug: myscale-authentication
source_filename: myscale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/myscale-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Cluster username and password (from the MyScale Cloud console Connection Details)\n    supplied as HTTP Basic credentials.\n  sources:\n  - openapi/myscale-openapi.yml\n- name: clickhouseUserHeader\n  type: apiKey\n  in: header\n  parameter: X-ClickHouse-User\n  description: Cluster username, paired with X-ClickHouse-Key.\n  sources:\n  - openapi/myscale-openapi.yml\n- name: clickhouseKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-ClickHouse-Key\n  description: Cluster password, paired with X-ClickHouse-User.\n  sources:\n  - openapi/myscale-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myscale/refs/heads/main/authentication/myscale-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Vector Database
- SQL
- ClickHouse
- Vector Search
- Full-Text Search
- RAG
---
