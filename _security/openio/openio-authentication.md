---
api_key_in:
- header
auth_types:
- awsSignature
- swiftAuth
description: 'OpenIO SDS exposes object storage through an S3-compatible gateway and an OpenStack Swift-compatible gateway. Authentication is therefore whatever the chosen gateway protocol defines: AWS Signature (v2 and v4) for the S3 gateway, and Swift auth (Keystone / TempAuth) for the Swift gateway. There is no provider-published OpenAPI, so this profile is derived from the documentation rather than from a machine-readable security scheme.'
kind: authentication
layout: security
method: searched
name: Openio Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenIO secures its APIs with awsSignature and swiftAuth across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OpenIO
provider_slug: openio
scheme_count: 2
schemes:
- credentials: S3 access key id + secret access key
  detail: S3 gateway authenticates requests with AWS Signature Version 4 (and legacy Signature Version 2). Both path-style and host-style (virtual hosted) bucket addressing are supported.
  name: s3-aws-signature-v4
  scheme: aws-sigv4
  sources:
  - https://docs.openio.io/latest/source/arch-design/s3_compliancy.html
  type: awsSignature
- detail: Swift gateway authenticates via OpenStack Keystone tokens or TempAuth, per the OpenStack Swift API it is compatible with.
  name: swift-auth
  scheme: keystone-or-tempauth
  sources:
  - https://docs.openio.io/latest/source/user-guide/swiftapi.html
  type: swiftAuth
slug: openio-authentication
source_filename: openio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.openio.io/latest/source/arch-design/iam.html\ndocs: https://docs.openio.io/latest/source/arch-design/iam.html\ndescription: >-\n  OpenIO SDS exposes object storage through an S3-compatible gateway and an\n  OpenStack Swift-compatible gateway. Authentication is therefore whatever the\n  chosen gateway protocol defines: AWS Signature (v2 and v4) for the S3 gateway,\n  and Swift auth (Keystone / TempAuth) for the Swift gateway. There is no\n  provider-published OpenAPI, so this profile is derived from the documentation\n  rather than from a machine-readable security scheme.\nsummary:\n  types: [awsSignature, swiftAuth]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: s3-aws-signature-v4\n    type: awsSignature\n    scheme: aws-sigv4\n    detail: >-\n      S3 gateway authenticates requests with AWS Signature Version 4 (and\n      legacy Signature Version 2). Both path-style and host-style (virtual\n\
  \      hosted) bucket addressing are supported.\n    credentials: S3 access key id + secret access key\n    sources: [https://docs.openio.io/latest/source/arch-design/s3_compliancy.html]\n  - name: swift-auth\n    type: swiftAuth\n    scheme: keystone-or-tempauth\n    detail: >-\n      Swift gateway authenticates via OpenStack Keystone tokens or TempAuth,\n      per the OpenStack Swift API it is compatible with.\n    sources: [https://docs.openio.io/latest/source/user-guide/swiftapi.html]\niam:\n  available: true\n  plan: paid\n  model: subset of AWS IAM applied at the S3 gateway\n  policy_scope: user policies only (bucket/resource policies not supported)\n  supported_actions:\n    - CreateBucket\n    - DeleteBucket\n    - GetBucketLocation\n    - ListBucket\n    - ListBucketMultipartUploads\n    - GetObject\n    - PutObject\n    - DeleteObject\n    - AbortMultipartUpload\n    - ListMultipartUploadParts\n  condition_keys: [s3:prefix, s3:delimiter, s3:max-keys]\n  operators: [StringEquals,\
  \ StringLike, StringNotEquals, StringNotLike]\n  admin_command: openio-admin iam set-user-policy\n  docs: https://docs.openio.io/latest/source/arch-design/iam.html\nnotes: >-\n  OpenIO SDS is self-hosted software (acquired by OVHcloud in 2020); the S3/Swift\n  gateway endpoint is deployment-specific, so there is no single hosted base URL.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openio/refs/heads/main/authentication/openio-authentication.yml
summary_line: awsSignature/swiftAuth · 2 schemes
tags:
- Company
- Infrastructure Saas
- Object Storage
- S3
- Cloud Storage
- Open Source
- OpenStack Swift
- Storage
---
