---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cassandra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Cassandra secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Cassandra
provider_slug: cassandra
scheme_count: 1
schemes:
- in: header
  name: cassandraToken
  parameter: X-Cassandra-Token
  sources:
  - openapi/cassandra-openapi.yml
  type: apiKey
slug: cassandra-authentication
source_filename: cassandra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cassandra-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: cassandraToken\n  type: apiKey\n  in: header\n  parameter: X-Cassandra-Token\n  sources:\n  - openapi/cassandra-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cassandra/refs/heads/main/authentication/cassandra-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Apache
- Big Data
- Database
- Distributed
- NoSQL
- Open Source
---
