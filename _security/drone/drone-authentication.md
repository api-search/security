---
api_key_in: []
api_specs:
- filename: drone-builds-api-openapi.yml
  format: yaml
  label: Drone Builds API
  slug: drone-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drone/refs/heads/main/openapi/drone-builds-api-openapi.yml
- filename: drone-cron-api-openapi.yml
  format: yaml
  label: Drone Cron API
  slug: drone-cron-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drone/refs/heads/main/openapi/drone-cron-api-openapi.yml
- filename: drone-nodes-api-openapi.yml
  format: yaml
  label: Drone Nodes API
  slug: drone-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drone/refs/heads/main/openapi/drone-nodes-api-openapi.yml
- filename: drone-queue-api-openapi.yml
  format: yaml
  label: Drone Queue API
  slug: drone-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drone/refs/heads/main/openapi/drone-queue-api-openapi.yml
- filename: drone-repos-api-openapi.yml
  format: yaml
  label: Drone Repos API
  slug: drone-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drone/refs/heads/main/openapi/drone-repos-api-openapi.yml
- filename: drone-secrets-api-openapi.yml
  format: yaml
  label: Drone Secrets API
  slug: drone-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drone/refs/heads/main/openapi/drone-secrets-api-openapi.yml
- filename: drone-system-api-openapi.yml
  format: yaml
  label: Drone System API
  slug: drone-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drone/refs/heads/main/openapi/drone-system-api-openapi.yml
- filename: drone-templates-api-openapi.yml
  format: yaml
  label: Drone Templates API
  slug: drone-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drone/refs/heads/main/openapi/drone-templates-api-openapi.yml
- filename: drone-user-api-openapi.yml
  format: yaml
  label: Drone User API
  slug: drone-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drone/refs/heads/main/openapi/drone-user-api-openapi.yml
- filename: drone-users-api-openapi.yml
  format: yaml
  label: Drone Users API
  slug: drone-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drone/refs/heads/main/openapi/drone-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Drone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Drone secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Drone
provider_slug: drone
scheme_count: 1
schemes:
- description: Bearer token retrieved from the Drone user interface profile page.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/drone-api-openapi.yml
  type: http
slug: drone-authentication
source_filename: drone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drone-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token retrieved from the Drone user interface profile page.\n  sources:\n  - openapi/drone-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drone/refs/heads/main/authentication/drone-authentication.yml
summary_line: http · 1 scheme
tags:
- CI/CD
- Continuous Integration
- Continuous Delivery
- DevOps
- Containers
- Docker
- Build Automation
- Open-Source
- Self-Hosted
---
