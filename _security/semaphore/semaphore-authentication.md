---
api_key_in: []
api_specs:
- filename: semaphore-semaphore-api-openapi.yml
  format: yaml
  label: Semaphore API
  slug: semaphore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/openapi/semaphore-semaphore-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Semaphore Authentication
name_suffix: Authentication
oauth_flows: []
overview: Semaphore secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Semaphore
provider_slug: semaphore
scheme_count: 1
schemes:
- description: Token that you get from semaphore [account settings](https://me.semaphoreci.com/account).
  name: authorization
  scheme: bearer
  sources:
  - openapi/semaphore-semaphore-api-openapi.yml
  type: http
slug: semaphore-authentication
source_filename: semaphore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/semaphore-semaphore-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: authorization\n  type: http\n  scheme: bearer\n  description: Token that you get from semaphore [account settings](https://me.semaphoreci.com/account).\n  sources:\n  - openapi/semaphore-semaphore-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semaphore/refs/heads/main/authentication/semaphore-authentication.yml
summary_line: http · 1 scheme
tags:
- CI/CD
- Continuous Integration
- Continuous Delivery
- Pipelines
- Workflows
- DevOps
- Build Automation
- Software Delivery
- Deployment
- Artifacts
---
