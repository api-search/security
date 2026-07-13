---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dagger Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dagger secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dagger
provider_slug: dagger
scheme_count: 1
schemes:
- description: 'HTTP Basic auth where the username is the value of the

    DAGGER_SESSION_TOKEN environment variable and the password is empty.'
  name: SessionTokenBasic
  scheme: basic
  sources:
  - openapi/dagger-openapi.yml
  type: http
slug: dagger-authentication
source_filename: dagger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dagger-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: SessionTokenBasic\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic auth where the username is the value of the\n    DAGGER_SESSION_TOKEN environment variable and the password is empty.\n  sources:\n  - openapi/dagger-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dagger/refs/heads/main/authentication/dagger-authentication.yml
summary_line: http · 1 scheme
tags:
- Build Automation
- BuildKit
- CI/CD
- Containers
- DAG
- Daggerverse
- DevOps
- GraphQL
- Modules
- OCI
- Open Source
- Pipelines
- Programmable Pipelines
- SDKs
---
