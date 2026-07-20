---
api_key_in: []
api_specs:
- filename: hcp-terraform-openapi.yml
  format: yaml
  label: HCP Terraform API
  slug: hcp-terraform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/openapi/hcp-terraform-openapi.yml
- filename: terraform-registry-openapi.yml
  format: yaml
  label: Terraform Registry API
  slug: terraform-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/openapi/terraform-registry-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Terraform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Terraform secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Terraform
provider_slug: terraform
scheme_count: 1
schemes:
- description: 'Bearer token authentication. HCP Terraform issues three token kinds — user tokens (act as a user), team tokens (scoped to a team''s permissions), and organization tokens (one per org, for org-level automation). Tokens are sent as `Authorization: Bearer <token>`. The public Terraform Registry API needs no authentication for discovery/download.'
  docs: https://developer.hashicorp.com/terraform/cloud-docs/users-teams-organizations/api-tokens
  header: Authorization
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hcp-terraform-openapi.yml
  token_types:
  - user
  - team
  - organization
  type: http
slug: terraform-authentication
source_filename: terraform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/hcp-terraform-openapi.yml\ndocs: https://developer.hashicorp.com/terraform/cloud-docs/users-teams-organizations/api-tokens\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token authentication. HCP Terraform issues three token kinds — user\n    tokens (act as a user), team tokens (scoped to a team's permissions), and\n    organization tokens (one per org, for org-level automation). Tokens are sent\n    as `Authorization: Bearer <token>`. The public Terraform Registry API needs\n    no authentication for discovery/download.\n  token_types: [user, team, organization]\n  header: Authorization\n  docs: https://developer.hashicorp.com/terraform/cloud-docs/users-teams-organizations/api-tokens\n  sources:\n  - openapi/hcp-terraform-openapi.yml\nnotes: >-\n  The Terraform Registry API (registry.terraform.io) is unauthenticated\
  \ for\n  public module/provider read and download. HCP Terraform also acts as an OIDC\n  identity provider (well-known/terraform-app-openid-configuration.json) for\n  workload identity / dynamic provider credentials — that is token issuance for\n  runs, distinct from API authentication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/authentication/terraform-authentication.yml
summary_line: http · 1 scheme
tags:
- Infrastructure As Code
- Cloud Infrastructure
- DevOps
- Open Source
- HashiCorp
---
