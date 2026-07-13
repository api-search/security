---
api_key_in:
- header
api_specs:
- filename: tigris-data-openapi.yml
  format: yaml
  label: Tigris Object Storage (S3-Compatible) API
  slug: object-storage-s3-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/openapi/tigris-data-openapi.yml
- filename: tigris-data-openapi.yml
  format: yaml
  label: Tigris Bucket Management API
  slug: bucket-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/openapi/tigris-data-openapi.yml
- filename: tigris-data-openapi.yml
  format: yaml
  label: Tigris Multipart Upload API
  slug: multipart-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/openapi/tigris-data-openapi.yml
- filename: tigris-data-openapi.yml
  format: yaml
  label: Tigris Presigned URLs API
  slug: presigned-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/openapi/tigris-data-openapi.yml
- filename: tigris-data-openapi.yml
  format: yaml
  label: Tigris IAM and Access Keys API
  slug: iam-access-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/openapi/tigris-data-openapi.yml
- filename: tigris-data-openapi.yml
  format: yaml
  label: Tigris Object Tiering API
  slug: object-tiering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/openapi/tigris-data-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tigris Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tigris secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tigris
provider_slug: tigris-data
scheme_count: 1
schemes:
- description: AWS Signature Version 4 request signing. Clients sign each request with a Tigris access key id (AWS_ACCESS_KEY_ID=tid_...) and secret access key (AWS_SECRET_ACCESS_KEY=tsec_...); the signature is carried in the standard Authorization header (or query string for presigned URLs). Use service name "s3" and region "auto". Any AWS SDK / SigV4 signer produces a compatible signature.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/tigris-data-openapi.yml
  type: apiKey
slug: tigris-data-authentication
source_filename: tigris-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tigris-data-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 request signing. Clients sign each request with a Tigris\n    access key id (AWS_ACCESS_KEY_ID=tid_...) and secret access key (AWS_SECRET_ACCESS_KEY=tsec_...);\n    the signature is carried in the standard Authorization header (or query string for presigned\n    URLs). Use service name \"s3\" and region \"auto\". Any AWS SDK / SigV4 signer produces a compatible\n    signature.\n  sources:\n  - openapi/tigris-data-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/authentication/tigris-data-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Object Storage
- S3 Compatible
- Storage
- Multi-Cloud
- Globally Distributed
---
