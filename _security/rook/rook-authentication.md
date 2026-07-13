---
api_key_in:
- header
api_specs:
- filename: rook-ceph-object-storage-openapi.yml
  format: yaml
  label: Rook Ceph Object Storage API
  slug: rook-ceph-object-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rook/refs/heads/main/openapi/rook-ceph-object-storage-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rook Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rook secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rook
provider_slug: rook
scheme_count: 1
schemes:
- description: AWS Signature Version 4 (SigV4) or AWS Signature Version 2 authentication using access key and secret key pairs provisioned by CephObjectStoreUser Kubernetes CRDs. Credentials are available in the Kubernetes Secret created by Rook for each CephObjectStoreUser.
  in: header
  name: s3Auth
  parameter: Authorization
  sources:
  - openapi/rook-ceph-object-storage-openapi.yml
  type: apiKey
slug: rook-authentication
source_filename: rook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rook-ceph-object-storage-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: s3Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 (SigV4) or AWS Signature Version 2 authentication using\n    access key and secret key pairs provisioned by CephObjectStoreUser Kubernetes CRDs. Credentials\n    are available in the Kubernetes Secret created by Rook for each CephObjectStoreUser.\n  sources:\n  - openapi/rook-ceph-object-storage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rook/refs/heads/main/authentication/rook-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Block Storage
- CNCF
- Ceph
- Cloud Native
- File Storage
- Graduated
- Kubernetes
- Object Storage
- Orchestration
- Storage
---
