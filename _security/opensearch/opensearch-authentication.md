---
api_key_in: []
api_specs:
- filename: opensearch-security-openapi.yml
  format: yaml
  label: OpenSearch Security Plugin REST API
  slug: opensearch-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/openapi/opensearch-security-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Opensearch Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenSearch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenSearch
provider_slug: opensearch
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/opensearch-security-openapi.yml
  type: http
slug: opensearch-authentication
source_filename: opensearch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/opensearch-security-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/opensearch-security-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensearch/refs/heads/main/authentication/opensearch-authentication.yml
summary_line: http · 1 scheme
tags:
- Search
- Analytics
- Observability
- Open Source
- Security
---
