---
api_key_in: []
api_specs:
- filename: maven-search-openapi.yml
  format: yaml
  label: Maven Central Search API
  slug: maven-central-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven/refs/heads/main/openapi/maven-search-openapi.yml
- filename: maven-portal-openapi.yml
  format: yaml
  label: Maven Central Portal Publishing API
  slug: maven-central-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven/refs/heads/main/openapi/maven-portal-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Maven Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maven secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Maven
provider_slug: maven
scheme_count: 1
schemes:
- description: Authorization header `Bearer <base64(username:password)>` using a user token generated from the Central Portal account settings.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/maven-portal-openapi.yml
  type: http
slug: maven-authentication
source_filename: maven-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/maven-portal-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Authorization header `Bearer <base64(username:password)>` using a user token\n    generated from the Central Portal account settings.\n  sources:\n  - openapi/maven-portal-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maven/refs/heads/main/authentication/maven-authentication.yml
summary_line: http · 1 scheme
tags:
- Artifacts
- Build Tools
- Java
- Maven
- Package Management
- Repository
---
