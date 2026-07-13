---
api_key_in:
- cookie
api_specs:
- filename: apache-couchdb-http-api-openapi.yaml
  format: yaml
  label: Apache CouchDB HTTP API
  slug: apache-couchdb-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/openapi/apache-couchdb-http-api-openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Couchdb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache CouchDB secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Apache CouchDB
provider_slug: apache-couchdb
scheme_count: 2
schemes:
- description: HTTP Basic authentication using CouchDB admin credentials
  name: basicAuth
  scheme: basic
  sources:
  - openapi/apache-couchdb-http-api-openapi.yaml
  type: http
- description: Cookie-based session authentication obtained via POST /_session
  in: cookie
  name: cookieAuth
  parameter: AuthSession
  sources:
  - openapi/apache-couchdb-http-api-openapi.yaml
  type: apiKey
slug: apache-couchdb-authentication
source_filename: apache-couchdb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-couchdb-http-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using CouchDB admin credentials\n  sources:\n  - openapi/apache-couchdb-http-api-openapi.yaml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: AuthSession\n  description: Cookie-based session authentication obtained via POST /_session\n  sources:\n  - openapi/apache-couchdb-http-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/authentication/apache-couchdb-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
---
