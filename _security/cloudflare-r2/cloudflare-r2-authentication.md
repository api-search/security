---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Cloudflare R2 S3-Compatible API
  slug: cloudflare-r2-s3-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/cloudflare/api-schemas/refs/heads/main/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Cloudflare R2 Cloudflare API
  slug: cloudflare-r2-cloudflare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/cloudflare/api-schemas/refs/heads/main/openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cloudflare R2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudflare R2 secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cloudflare R2
provider_slug: cloudflare-r2
scheme_count: 5
schemes:
- in: header
  name: api_email
  parameter: X-Auth-Email
  sources:
  - openapi/cloudflare-r2-cloudflare-api-openapi.yml
  type: apiKey
- in: header
  name: api_key
  parameter: X-Auth-Key
  sources:
  - openapi/cloudflare-r2-cloudflare-api-openapi.yml
  type: apiKey
- name: api_token
  scheme: bearer
  sources:
  - openapi/cloudflare-r2-cloudflare-api-openapi.yml
  type: http
- in: header
  name: user_service_key
  parameter: X-Auth-User-Service-Key
  sources:
  - openapi/cloudflare-r2-cloudflare-api-openapi.yml
  type: apiKey
- description: AWS Signature Version 4 authentication. Use your R2 API token (Access Key ID and Secret Access Key) generated from the R2 dashboard. Compatible with all AWS S3 SDKs.
  in: header
  name: hmacAuth
  parameter: Authorization
  sources:
  - openapi/cloudflare-r2-s3-compatible-api-openapi.yml
  type: apiKey
slug: cloudflare-r2-authentication
source_filename: cloudflare-r2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudflare-r2-cloudflare-api-openapi.yml, openapi/cloudflare-r2-s3-compatible-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_email\n  type: apiKey\n  in: header\n  parameter: X-Auth-Email\n  sources:\n  - openapi/cloudflare-r2-cloudflare-api-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: X-Auth-Key\n  sources:\n  - openapi/cloudflare-r2-cloudflare-api-openapi.yml\n- name: api_token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/cloudflare-r2-cloudflare-api-openapi.yml\n- name: user_service_key\n  type: apiKey\n  in: header\n  parameter: X-Auth-User-Service-Key\n  sources:\n  - openapi/cloudflare-r2-cloudflare-api-openapi.yml\n- name: hmacAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 authentication. Use your R2 API token (Access Key ID\n    and Secret Access Key) generated\
  \ from the R2 dashboard. Compatible with all AWS S3 SDKs.\n  sources:\n  - openapi/cloudflare-r2-s3-compatible-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/authentication/cloudflare-r2-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Object Storage
- Cloud Storage
- S3-Compatible
- Egress-Free
- Buckets
- Developer Platform
- Cloudflare
---
