---
api_key_in:
- header
api_specs:
- filename: filebase-s3-api-openapi.yml
  format: yaml
  label: Filebase S3-Compatible API
  slug: filebase-s3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-s3-api-openapi.yml
- filename: filebase-platform-api-openapi.yml
  format: yaml
  label: Filebase Platform API
  slug: filebase-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-platform-api-openapi.yml
- filename: filebase-ipfs-pinning-service-api-openapi.yml
  format: yaml
  label: Filebase IPFS Pinning Service API
  slug: filebase-ipfs-pinning-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-ipfs-pinning-service-api-openapi.yml
- filename: filebase-ipfs-rpc-api-openapi.yml
  format: yaml
  label: Filebase IPFS RPC API
  slug: filebase-ipfs-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/filebase/refs/heads/main/openapi/filebase-ipfs-rpc-api-openapi.yml
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
