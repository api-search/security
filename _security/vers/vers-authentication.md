---
api_key_in: []
api_specs:
- filename: vers-commit-tags-api-openapi.yml
  format: yaml
  label: Vers commit_tags API
  slug: vers-commit-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-commit-tags-api-openapi.yml
- filename: vers-commits-api-openapi.yml
  format: yaml
  label: Vers commits API
  slug: vers-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-commits-api-openapi.yml
- filename: vers-deploy-api-openapi.yml
  format: yaml
  label: Vers deploy API
  slug: vers-deploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-deploy-api-openapi.yml
- filename: vers-domains-api-openapi.yml
  format: yaml
  label: Vers domains API
  slug: vers-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-domains-api-openapi.yml
- filename: vers-env-vars-api-openapi.yml
  format: yaml
  label: Vers env_vars API
  slug: vers-env-vars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-env-vars-api-openapi.yml
- filename: vers-images-api-openapi.yml
  format: yaml
  label: Vers images API
  slug: vers-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-images-api-openapi.yml
- filename: vers-keys-api-openapi.yml
  format: yaml
  label: Vers keys API
  slug: vers-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-keys-api-openapi.yml
- filename: vers-public-repositories-api-openapi.yml
  format: yaml
  label: Vers public_repositories API
  slug: vers-public-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-public-repositories-api-openapi.yml
- filename: vers-repositories-api-openapi.yml
  format: yaml
  label: Vers repositories API
  slug: vers-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-repositories-api-openapi.yml
- filename: vers-system-api-openapi.yml
  format: yaml
  label: Vers System API
  slug: vers-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-system-api-openapi.yml
- filename: vers-vm-api-openapi.yml
  format: yaml
  label: Vers vm API
  slug: vers-vm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-vm-api-openapi.yml
- filename: vers-vms-api-openapi.yml
  format: yaml
  label: Vers vms API
  slug: vers-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/openapi/vers-vms-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vers Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vers secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vers
provider_slug: vers
scheme_count: 1
schemes:
- bearerFormat: Token
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/vers-openapi-original.json
  type: http
slug: vers-authentication
source_filename: vers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/vers-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  bearerFormat: Token\n  sources:\n  - openapi/vers-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vers/refs/heads/main/authentication/vers-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Compute
- Virtualization
- MicroVM
- Orchestration
- Infrastructure
- AI Agents
- Developer Tools
- Sandbox
- CI/CD
---
