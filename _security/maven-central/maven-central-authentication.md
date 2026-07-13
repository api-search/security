---
api_key_in: []
api_specs:
- filename: maven-central-search-openapi.yml
  format: yaml
  label: Maven Central Search API
  slug: maven-central-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-central/refs/heads/main/openapi/maven-central-search-openapi.yml
- filename: maven-central-portal-openapi.yml
  format: yaml
  label: Central Portal Publishing API
  slug: central-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-central/refs/heads/main/openapi/maven-central-portal-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Maven Central Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maven Central secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Maven Central
provider_slug: maven-central
scheme_count: 1
schemes:
- description: Authorization header `Bearer <base64(username:password)>` using a user token generated from the Central Portal account settings.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/maven-central-portal-openapi.yml
  type: http
slug: maven-central-authentication
source_filename: maven-central-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/maven-central-portal-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Authorization header `Bearer <base64(username:password)>` using a user token\n    generated from the Central Portal account settings.\n  sources:\n  - openapi/maven-central-portal-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maven-central/refs/heads/main/authentication/maven-central-authentication.yml
summary_line: http · 1 scheme
tags:
- Artifacts
- Java
- JVM
- Maven
- Package Management
- Repository
---
