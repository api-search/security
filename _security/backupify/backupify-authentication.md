---
api_key_in: []
api_specs:
- filename: backupify-saas-protection-api.yaml
  format: yaml
  label: Backupify SaaS Protection API
  slug: saas-protection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/openapi/backupify-saas-protection-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Backupify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Backupify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Backupify
provider_slug: backupify
scheme_count: 1
schemes:
- description: HTTP Basic authentication using API public key as username and private key as password
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/backupify-saas-protection-api.yaml
  type: http
slug: backupify-authentication
source_filename: backupify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/backupify-saas-protection-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using API public key as username and private key as\n    password\n  sources:\n  - openapi/backupify-saas-protection-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/authentication/backupify-authentication.yml
summary_line: http · 1 scheme
tags:
- SaaS Backup
- Data Protection
- Cloud Backup
- Microsoft 365
- Google Workspace
---
