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
method: derived
name: Terraform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Terraform secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Terraform
provider_slug: terraform
scheme_count: 1
schemes:
- description: Bearer token authentication. Use organization, team, or user tokens.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hcp-terraform-openapi.yml
  type: http
slug: terraform-authentication
source_filename: terraform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hcp-terraform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication. Use organization, team, or user tokens.\n  sources:\n  - openapi/hcp-terraform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terraform/refs/heads/main/authentication/terraform-authentication.yml
summary_line: http · 1 scheme
tags:
- Infrastructure As Code
- Cloud Infrastructure
- DevOps
- Open Source
- HashiCorp
---
