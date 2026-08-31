---
api_key_in: []
api_specs:
- filename: dalcor-pharmaceuticals-categories-api-openapi.yml
  format: yaml
  label: DalCor Pharmaceuticals Categories API
  slug: dalcor-pharmaceuticals-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/openapi/dalcor-pharmaceuticals-categories-api-openapi.yml
- filename: dalcor-pharmaceuticals-comments-api-openapi.yml
  format: yaml
  label: DalCor Pharmaceuticals Comments API
  slug: dalcor-pharmaceuticals-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/openapi/dalcor-pharmaceuticals-comments-api-openapi.yml
- filename: dalcor-pharmaceuticals-discovery-api-openapi.yml
  format: yaml
  label: DalCor Pharmaceuticals Discovery API
  slug: dalcor-pharmaceuticals-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/openapi/dalcor-pharmaceuticals-discovery-api-openapi.yml
- filename: dalcor-pharmaceuticals-media-api-openapi.yml
  format: yaml
  label: DalCor Pharmaceuticals Media API
  slug: dalcor-pharmaceuticals-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/openapi/dalcor-pharmaceuticals-media-api-openapi.yml
- filename: dalcor-pharmaceuticals-pages-api-openapi.yml
  format: yaml
  label: DalCor Pharmaceuticals Pages API
  slug: dalcor-pharmaceuticals-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/openapi/dalcor-pharmaceuticals-pages-api-openapi.yml
- filename: dalcor-pharmaceuticals-posts-api-openapi.yml
  format: yaml
  label: DalCor Pharmaceuticals Posts API
  slug: dalcor-pharmaceuticals-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/openapi/dalcor-pharmaceuticals-posts-api-openapi.yml
- filename: dalcor-pharmaceuticals-search-api-openapi.yml
  format: yaml
  label: DalCor Pharmaceuticals Search API
  slug: dalcor-pharmaceuticals-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/openapi/dalcor-pharmaceuticals-search-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dalcor Pharmaceuticals Authentication
name_suffix: Authentication
oauth_flows: []
overview: DalCor Pharmaceuticals secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DalCor Pharmaceuticals
provider_slug: dalcor-pharmaceuticals
scheme_count: 1
schemes:
- description: WordPress Application Passwords (RFC 7617 Basic over TLS). Required only for write and administrative routes, which are out of scope for this document — every operation modelled here returns 200 anonymously.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/dalcor-pharmaceuticals-content-openapi.yml
  type: http
slug: dalcor-pharmaceuticals-authentication
source_filename: dalcor-pharmaceuticals-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: openapi/dalcor-pharmaceuticals-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords (RFC 7617 Basic over TLS). Required only for\n    write and administrative routes, which are out of scope for this document — every operation\n    modelled here returns 200 anonymously.\n  sources:\n  - openapi/dalcor-pharmaceuticals-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/authentication/dalcor-pharmaceuticals-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- pharmaceuticals
- biotechnology
- cardiovascular
- precision-medicine
- pharmacogenomics
- clinical-trials
- life-sciences
- content-api
---
