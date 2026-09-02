---
api_key_in:
- header
api_specs:
- filename: cloudflare-r2-buckets-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Buckets API
  slug: cloudflare-r2-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-buckets-api-openapi.yml
- filename: cloudflare-r2-cors-api-openapi.yml
  format: yaml
  label: Cloudflare R2 CORS API
  slug: cloudflare-r2-cors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-cors-api-openapi.yml
- filename: cloudflare-r2-credential-management-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Credential Management API
  slug: cloudflare-r2-credential-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-credential-management-api-openapi.yml
- filename: cloudflare-r2-lifecycle-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Lifecycle API
  slug: cloudflare-r2-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-lifecycle-api-openapi.yml
- filename: cloudflare-r2-maintenance-configuration-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Maintenance Configuration API
  slug: cloudflare-r2-maintenance-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-maintenance-configuration-api-openapi.yml
- filename: cloudflare-r2-multipart-upload-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Multipart Upload API
  slug: cloudflare-r2-multipart-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-multipart-upload-api-openapi.yml
- filename: cloudflare-r2-namespace-management-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Namespace Management API
  slug: cloudflare-r2-namespace-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-namespace-management-api-openapi.yml
- filename: cloudflare-r2-objects-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Objects API
  slug: cloudflare-r2-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-objects-api-openapi.yml
- filename: cloudflare-r2-r2-account-api-openapi.yml
  format: yaml
  label: Cloudflare R2 R2 Account API
  slug: cloudflare-r2-r2-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-r2-account-api-openapi.yml
- filename: cloudflare-r2-r2-bucket-api-openapi.yml
  format: yaml
  label: Cloudflare R2 R2 Bucket API
  slug: cloudflare-r2-r2-bucket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-r2-bucket-api-openapi.yml
- filename: cloudflare-r2-r2-catalog-management-api-openapi.yml
  format: yaml
  label: Cloudflare R2 R2 Catalog Management API
  slug: cloudflare-r2-r2-catalog-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-r2-catalog-management-api-openapi.yml
- filename: cloudflare-r2-r2-object-api-openapi.yml
  format: yaml
  label: Cloudflare R2 R2 Object API
  slug: cloudflare-r2-r2-object-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-r2-object-api-openapi.yml
- filename: cloudflare-r2-table-maintenance-configuration-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Table Maintenance Configuration API
  slug: cloudflare-r2-table-maintenance-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-table-maintenance-configuration-api-openapi.yml
- filename: cloudflare-r2-table-management-api-openapi.yml
  format: yaml
  label: Cloudflare R2 Table Management API
  slug: cloudflare-r2-table-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudflare-r2/refs/heads/main/openapi/cloudflare-r2-table-management-api-openapi.yml
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
- S3 Compatible
- Egress-Free
- Buckets
- Developer Platform
- Cloudflare
---
