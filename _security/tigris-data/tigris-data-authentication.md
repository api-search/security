---
api_key_in:
- header
api_specs:
- filename: tigris-data-buckets-api-openapi.yml
  format: yaml
  label: Tigris Buckets API
  slug: tigris-data-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/openapi/tigris-data-buckets-api-openapi.yml
- filename: tigris-data-multipart-api-openapi.yml
  format: yaml
  label: Tigris Multipart API
  slug: tigris-data-multipart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/openapi/tigris-data-multipart-api-openapi.yml
- filename: tigris-data-objects-api-openapi.yml
  format: yaml
  label: Tigris Objects API
  slug: tigris-data-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigris-data/refs/heads/main/openapi/tigris-data-objects-api-openapi.yml
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
