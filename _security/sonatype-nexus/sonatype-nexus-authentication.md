---
api_key_in: []
api_specs:
- filename: sonatype-nexus-repository-openapi.yml
  format: yaml
  label: Nexus Repository API
  slug: nexus-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sonatype-nexus/refs/heads/main/openapi/sonatype-nexus-repository-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sonatype Nexus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sonatype Nexus secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sonatype Nexus
provider_slug: sonatype-nexus
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/sonatype-nexus-repository-openapi.yml
  type: http
slug: sonatype-nexus-authentication
source_filename: sonatype-nexus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sonatype-nexus-repository-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/sonatype-nexus-repository-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonatype-nexus/refs/heads/main/authentication/sonatype-nexus-authentication.yml
summary_line: http · 1 scheme
tags:
- Artifact Management
- DevOps
- Package Management
- Repository
- Maven
- npm
- Docker
- Software Supply Chain
---
