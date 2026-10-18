---
anonymous_access: false
api_key_in: []
api_specs:
- filename: rustfs-health-api-openapi.yml
  format: yaml
  label: RustFS Health API
  slug: rustfs-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rustfs/refs/heads/main/openapi/rustfs-health-api-openapi.yml
- filename: rustfs-minio-api-openapi.yml
  format: yaml
  label: RustFS Minio API
  slug: rustfs-minio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rustfs/refs/heads/main/openapi/rustfs-minio-api-openapi.yml
- filename: rustfs-rustfs-api-api-openapi.yml
  format: yaml
  label: RustFS RustFS API
  slug: rustfs-rustfs-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rustfs/refs/heads/main/openapi/rustfs-rustfs-api-api-openapi.yml
- filename: rustfs-rustfs-api-openapi.yml
  format: yaml
  label: RustFS Rustfs API
  slug: rustfs-rustfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rustfs/refs/heads/main/openapi/rustfs-rustfs-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Rustfs Authentication
name_suffix: Authentication
oauth_flows: []
overview: RustFS declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: RustFS
provider_slug: rustfs
scheme_count: 3
schemes:
- credentials: RUSTFS_ACCESS_KEY / RUSTFS_SECRET_KEY (root), plus IAM users and service accounts
  description: S3 and admin requests are signed with AWS SigV4 using an access key and secret key; the access key is embedded in the slash-delimited SigV4 credential scope, so RUSTFS_ACCESS_KEY must not contain '/'.
  name: AWS Signature Version 4
  scheme: aws-sigv4
  type: http
- description: Security Token Service (POST / on the S3 port) issues temporary credentials, including AssumeRoleWithWebIdentity for OIDC identity providers.
  name: STS temporary credentials
  type: sts
- description: External OIDC identity providers (for example Keycloak) can be configured for console login and STS.
  name: OpenID Connect
  type: openIdConnect
slug: rustfs-authentication
source_filename: rustfs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: RustFS Authentication\ngenerated: '2026-10-14'\nmethod: searched\nsource:\n- https://docs.rustfs.com/en/operations/credentials\n- https://docs.rustfs.com/en/security-compliance/iam/sts\n- https://docs.rustfs.com/en/security-compliance/oidc\nschemes:\n- name: AWS Signature Version 4\n  type: http\n  scheme: aws-sigv4\n  description: S3 and admin requests are signed with AWS SigV4 using an access key and secret key; the access key is embedded in the slash-delimited SigV4 credential scope, so RUSTFS_ACCESS_KEY must not contain '/'.\n  credentials: RUSTFS_ACCESS_KEY / RUSTFS_SECRET_KEY (root), plus IAM users and service accounts\n- name: STS temporary credentials\n  type: sts\n  description: Security Token Service (POST / on the S3 port) issues temporary credentials, including AssumeRoleWithWebIdentity for OIDC identity providers.\n- name: OpenID Connect\n  type: openIdConnect\n  description: External OIDC identity providers (for example Keycloak) can be configured for console\
  \ login and STS.\nnotes: The default secret key rustfsadmin is publicly known; internode RPC secret derivation fails closed when it is used.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rustfs/refs/heads/main/authentication/rustfs-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Object Storage
- S3
- Open Source
- Storage
---
