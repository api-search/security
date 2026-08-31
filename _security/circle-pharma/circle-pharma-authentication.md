---
api_key_in: []
api_specs:
- filename: circle-pharma-categories-api-openapi.yml
  format: yaml
  label: Circle Pharma Categories API
  slug: circle-pharma-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-categories-api-openapi.yml
- filename: circle-pharma-comments-api-openapi.yml
  format: yaml
  label: Circle Pharma Comments API
  slug: circle-pharma-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-comments-api-openapi.yml
- filename: circle-pharma-discovery-api-openapi.yml
  format: yaml
  label: Circle Pharma Discovery API
  slug: circle-pharma-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-discovery-api-openapi.yml
- filename: circle-pharma-events-api-openapi.yml
  format: yaml
  label: Circle Pharma Events API
  slug: circle-pharma-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-events-api-openapi.yml
- filename: circle-pharma-media-api-openapi.yml
  format: yaml
  label: Circle Pharma Media API
  slug: circle-pharma-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-media-api-openapi.yml
- filename: circle-pharma-pages-api-openapi.yml
  format: yaml
  label: Circle Pharma Pages API
  slug: circle-pharma-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-pages-api-openapi.yml
- filename: circle-pharma-posts-api-openapi.yml
  format: yaml
  label: Circle Pharma Posts API
  slug: circle-pharma-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-posts-api-openapi.yml
- filename: circle-pharma-search-api-openapi.yml
  format: yaml
  label: Circle Pharma Search API
  slug: circle-pharma-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-search-api-openapi.yml
- filename: circle-pharma-tags-api-openapi.yml
  format: yaml
  label: Circle Pharma Tags API
  slug: circle-pharma-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-tags-api-openapi.yml
- filename: circle-pharma-team-api-openapi.yml
  format: yaml
  label: Circle Pharma Team API
  slug: circle-pharma-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/openapi/circle-pharma-team-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Circle Pharma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Circle Pharma secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Circle Pharma
provider_slug: circle-pharma
scheme_count: 1
schemes:
- description: WordPress Application Passwords (RFC 7617 Basic over TLS). Required only for write and administrative routes, which are out of scope for this document — every operation modelled here is anonymous.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/circle-pharma-content-openapi.yml
  type: http
slug: circle-pharma-authentication
source_filename: circle-pharma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: derived\nsource: openapi/circle-pharma-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords (RFC 7617 Basic over TLS). Required only for\n    write and administrative routes, which are out of scope for this document — every operation\n    modelled here is anonymous.\n  sources:\n  - openapi/circle-pharma-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circle-pharma/refs/heads/main/authentication/circle-pharma-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- biotechnology
- pharmaceuticals
- oncology
- drug-discovery
- macrocycles
- clinical-trials
- life-sciences
- content-api
---
