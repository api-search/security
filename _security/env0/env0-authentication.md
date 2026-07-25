---
api_key_in: []
api_specs:
- filename: env0-agents-api-openapi.yml
  format: yaml
  label: Env0 Agents API
  slug: env0-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-agents-api-openapi.yml
- filename: env0-approvalpolicies-api-openapi.yml
  format: yaml
  label: Env0 ApprovalPolicies API
  slug: env0-approvalpolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-approvalpolicies-api-openapi.yml
- filename: env0-configuration-api-openapi.yml
  format: yaml
  label: Env0 Configuration API
  slug: env0-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-configuration-api-openapi.yml
- filename: env0-deployments-api-openapi.yml
  format: yaml
  label: Env0 Deployments API
  slug: env0-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-deployments-api-openapi.yml
- filename: env0-environments-api-openapi.yml
  format: yaml
  label: Env0 Environments API
  slug: env0-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-environments-api-openapi.yml
- filename: env0-modules-api-openapi.yml
  format: yaml
  label: Env0 Modules API
  slug: env0-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-modules-api-openapi.yml
- filename: env0-organizations-api-openapi.yml
  format: yaml
  label: Env0 Organizations API
  slug: env0-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-organizations-api-openapi.yml
- filename: env0-projects-api-openapi.yml
  format: yaml
  label: Env0 Projects API
  slug: env0-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-projects-api-openapi.yml
- filename: env0-templates-api-openapi.yml
  format: yaml
  label: Env0 Templates API
  slug: env0-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-templates-api-openapi.yml
- filename: env0-users-api-openapi.yml
  format: yaml
  label: Env0 Users API
  slug: env0-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-users-api-openapi.yml
- filename: env0-webhooks-api-openapi.yml
  format: yaml
  label: Env0 Webhooks API
  slug: env0-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Env0 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Env0 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Env0
provider_slug: env0
scheme_count: 1
schemes:
- description: HTTP Basic Authentication. Username is the env0 API Key ID and the password is the API Key Secret, both created in the env0 organization settings.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/env0-openapi.yml
  type: http
slug: env0-authentication
source_filename: env0-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/env0-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication. Username is the env0 API Key ID and the password is\n    the API Key Secret, both created in the env0 organization settings.\n  sources:\n  - openapi/env0-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/authentication/env0-authentication.yml
summary_line: http · 1 scheme
tags:
- FinOps
- Infrastructure as Code
- DevOps
- Cloud
---
