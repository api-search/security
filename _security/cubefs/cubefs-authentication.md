---
api_key_in:
- header
api_specs:
- filename: cubefs-acls-api-openapi.yml
  format: yaml
  label: CubeFS ACLs API
  slug: cubefs-acls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-acls-api-openapi.yml
- filename: cubefs-buckets-api-openapi.yml
  format: yaml
  label: CubeFS Buckets API
  slug: cubefs-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-buckets-api-openapi.yml
- filename: cubefs-cluster-api-openapi.yml
  format: yaml
  label: CubeFS Cluster API
  slug: cubefs-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-cluster-api-openapi.yml
- filename: cubefs-datanodes-api-openapi.yml
  format: yaml
  label: CubeFS DataNodes API
  slug: cubefs-datanodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-datanodes-api-openapi.yml
- filename: cubefs-datapartitions-api-openapi.yml
  format: yaml
  label: CubeFS DataPartitions API
  slug: cubefs-datapartitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-datapartitions-api-openapi.yml
- filename: cubefs-metanodes-api-openapi.yml
  format: yaml
  label: CubeFS MetaNodes API
  slug: cubefs-metanodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-metanodes-api-openapi.yml
- filename: cubefs-metapartitions-api-openapi.yml
  format: yaml
  label: CubeFS MetaPartitions API
  slug: cubefs-metapartitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-metapartitions-api-openapi.yml
- filename: cubefs-multipart-api-openapi.yml
  format: yaml
  label: CubeFS Multipart API
  slug: cubefs-multipart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-multipart-api-openapi.yml
- filename: cubefs-objects-api-openapi.yml
  format: yaml
  label: CubeFS Objects API
  slug: cubefs-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-objects-api-openapi.yml
- filename: cubefs-users-api-openapi.yml
  format: yaml
  label: CubeFS Users API
  slug: cubefs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-users-api-openapi.yml
- filename: cubefs-volumes-api-openapi.yml
  format: yaml
  label: CubeFS Volumes API
  slug: cubefs-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-volumes-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cubefs Authentication
name_suffix: Authentication
oauth_flows: []
overview: CubeFS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CubeFS
provider_slug: cubefs
scheme_count: 1
schemes:
- description: 'AWS Signature Version 4 authorization. Format: AWS4-HMAC-SHA256 Credential={accessKey}/{date}/{region}/s3/aws4_request, SignedHeaders={headers}, Signature={signature}. Access keys are managed via the CubeFS Master API user management endpoints.'
  in: header
  name: awsAuth
  parameter: Authorization
  sources:
  - openapi/cubefs-s3-api-openapi.yml
  type: apiKey
slug: cubefs-authentication
source_filename: cubefs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cubefs-s3-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: awsAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'AWS Signature Version 4 authorization. Format: AWS4-HMAC-SHA256 Credential={accessKey}/{date}/{region}/s3/aws4_request,\n    SignedHeaders={headers}, Signature={signature}. Access keys are managed via the CubeFS Master\n    API user management endpoints.'\n  sources:\n  - openapi/cubefs-s3-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/authentication/cubefs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud-Native
- CNCF Graduated
- Distributed File System
- Kubernetes
- Object Storage
- POSIX
- S3 Compatible
- Storage
---
