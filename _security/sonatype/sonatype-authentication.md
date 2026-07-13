---
api_key_in: []
api_specs:
- filename: sonatype-lifecycle-openapi.yml
  format: yaml
  label: Sonatype Lifecycle API
  slug: sonatype-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonatype/refs/heads/main/openapi/sonatype-lifecycle-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sonatype Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sonatype secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Sonatype
provider_slug: sonatype
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/sonatype-lifecycle-openapi.yml
  type: http
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sonatype-lifecycle-openapi.yml
  type: http
slug: sonatype-authentication
source_filename: sonatype-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sonatype-lifecycle-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/sonatype-lifecycle-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/sonatype-lifecycle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonatype/refs/heads/main/authentication/sonatype-authentication.yml
summary_line: http · 2 schemes
tags:
- Software Supply Chain
- Security
- Vulnerability Management
- SBOM
- Software Composition Analysis
- DevSecOps
---
