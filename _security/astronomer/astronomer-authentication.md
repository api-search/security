---
api_key_in: []
api_specs:
- filename: astronomer-agenttoken-api-openapi.yml
  format: yaml
  label: Astronomer AgentToken API
  slug: astronomer-agenttoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-agenttoken-api-openapi.yml
- filename: astronomer-allowedipaddressrange-api-openapi.yml
  format: yaml
  label: Astronomer AllowedIpAddressRange API
  slug: astronomer-allowedipaddressrange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-allowedipaddressrange-api-openapi.yml
- filename: astronomer-apitoken-api-openapi.yml
  format: yaml
  label: Astronomer ApiToken API
  slug: astronomer-apitoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-apitoken-api-openapi.yml
- filename: astronomer-authorization-api-openapi.yml
  format: yaml
  label: Astronomer Authorization API
  slug: astronomer-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-authorization-api-openapi.yml
- filename: astronomer-cluster-api-openapi.yml
  format: yaml
  label: Astronomer Cluster API
  slug: astronomer-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-cluster-api-openapi.yml
- filename: astronomer-deploy-api-openapi.yml
  format: yaml
  label: Astronomer Deploy API
  slug: astronomer-deploy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-deploy-api-openapi.yml
- filename: astronomer-deployment-api-openapi.yml
  format: yaml
  label: Astronomer Deployment API
  slug: astronomer-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-deployment-api-openapi.yml
- filename: astronomer-environment-api-openapi.yml
  format: yaml
  label: Astronomer Environment API
  slug: astronomer-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-environment-api-openapi.yml
- filename: astronomer-invite-api-openapi.yml
  format: yaml
  label: Astronomer Invite API
  slug: astronomer-invite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-invite-api-openapi.yml
- filename: astronomer-options-api-openapi.yml
  format: yaml
  label: Astronomer Options API
  slug: astronomer-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-options-api-openapi.yml
- filename: astronomer-organization-api-openapi.yml
  format: yaml
  label: Astronomer Organization API
  slug: astronomer-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-organization-api-openapi.yml
- filename: astronomer-role-api-openapi.yml
  format: yaml
  label: Astronomer Role API
  slug: astronomer-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-role-api-openapi.yml
- filename: astronomer-team-api-openapi.yml
  format: yaml
  label: Astronomer Team API
  slug: astronomer-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-team-api-openapi.yml
- filename: astronomer-user-api-openapi.yml
  format: yaml
  label: Astronomer User API
  slug: astronomer-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-user-api-openapi.yml
- filename: astronomer-workspace-api-openapi.yml
  format: yaml
  label: Astronomer Workspace API
  slug: astronomer-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/openapi/astronomer-workspace-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Astronomer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Astronomer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Astronomer
provider_slug: astronomer
scheme_count: 1
schemes:
- name: JWT
  scheme: bearer
  sources:
  - openapi/astronomer-astro-openapi-original.yml
  type: http
slug: astronomer-authentication
source_filename: astronomer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/astronomer-astro-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: JWT\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/astronomer-astro-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astronomer/refs/heads/main/authentication/astronomer-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data Orchestration
- Apache Airflow
- Data Pipelines
- Data Engineering
- Workflow Automation
- MLOps
- Managed Platform
---
