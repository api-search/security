---
api_key_in:
- header
api_specs:
- filename: filebase-buckets-api-openapi.yml
  format: yaml
  label: Filebase Buckets API
  slug: filebase-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-buckets-api-openapi.yml
- filename: filebase-data-management-api-openapi.yml
  format: yaml
  label: Filebase Data Management API
  slug: filebase-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-data-management-api-openapi.yml
- filename: filebase-ipns-api-openapi.yml
  format: yaml
  label: Filebase IPNS API
  slug: filebase-ipns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-ipns-api-openapi.yml
- filename: filebase-keypairs-api-openapi.yml
  format: yaml
  label: Filebase Keypairs API
  slug: filebase-keypairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-keypairs-api-openapi.yml
- filename: filebase-mfs-api-openapi.yml
  format: yaml
  label: Filebase MFS API
  slug: filebase-mfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-mfs-api-openapi.yml
- filename: filebase-multipart-upload-api-openapi.yml
  format: yaml
  label: Filebase Multipart Upload API
  slug: filebase-multipart-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-multipart-upload-api-openapi.yml
- filename: filebase-node-api-openapi.yml
  format: yaml
  label: Filebase Node API
  slug: filebase-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-node-api-openapi.yml
- filename: filebase-objects-api-openapi.yml
  format: yaml
  label: Filebase Objects API
  slug: filebase-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-objects-api-openapi.yml
- filename: filebase-pinning-api-openapi.yml
  format: yaml
  label: Filebase Pinning API
  slug: filebase-pinning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-pinning-api-openapi.yml
- filename: filebase-pins-api-openapi.yml
  format: yaml
  label: Filebase Pins API
  slug: filebase-pins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-pins-api-openapi.yml
- filename: filebase-usage-api-openapi.yml
  format: yaml
  label: Filebase Usage API
  slug: filebase-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-usage-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Filebase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Filebase secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Filebase
provider_slug: filebase
scheme_count: 2
schemes:
- description: Per-bucket Bearer token for authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/filebase-ipfs-pinning-service-api-openapi.yml
  - openapi/filebase-ipfs-rpc-api-openapi.yml
  - openapi/filebase-platform-api-openapi.yml
  type: http
- description: AWS Signature Version 4 (AWS4-HMAC-SHA256) with Filebase access key and secret key. Use endpoint s3.filebase.io and region us-east-1.
  in: header
  name: AWS4Auth
  parameter: Authorization
  sources:
  - openapi/filebase-s3-api-openapi.yml
  type: apiKey
slug: filebase-authentication
source_filename: filebase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/filebase-ipfs-pinning-service-api-openapi.yml, openapi/filebase-ipfs-rpc-api-openapi.yml,\n  openapi/filebase-platform-api-openapi.yml, openapi/filebase-s3-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Per-bucket Bearer token for authentication\n  sources:\n  - openapi/filebase-ipfs-pinning-service-api-openapi.yml\n  - openapi/filebase-ipfs-rpc-api-openapi.yml\n  - openapi/filebase-platform-api-openapi.yml\n- name: AWS4Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 (AWS4-HMAC-SHA256) with Filebase access key and secret\n    key. Use endpoint s3.filebase.io and region us-east-1.\n  sources:\n  - openapi/filebase-s3-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/authentication/filebase-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Object Storage
- IPFS
- S3-Compatible
- Decentralized Storage
- Pinning
- Web3
- Cloud Storage
- Blockchain
---
