---
api_key_in: []
api_specs:
- filename: solr-openapi.yml
  format: yaml
  label: Apache Solr REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solr/refs/heads/main/openapi/solr-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Solr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Solr secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Solr
provider_slug: solr
scheme_count: 1
schemes:
- description: HTTP Basic Authentication (Solr Basic Auth plugin). JWT and certificate auth plugins are also supported.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/solr-openapi.yml
  type: http
slug: solr-authentication
source_filename: solr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/solr-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication (Solr Basic Auth plugin). JWT and certificate auth\n    plugins are also supported.\n  sources:\n  - openapi/solr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solr/refs/heads/main/authentication/solr-authentication.yml
summary_line: http · 1 scheme
tags:
- Search
- Enterprise Search
- Full-Text Search
- Open Source
- Lucene
- Indexing
---
