---
api_key_in:
- header
auth_types:
- signature-v4
- sts
- ldap
- oidc
description: ''
kind: authentication
layout: security
method: searched
name: Minio Authentication
name_suffix: Authentication
oauth_flows: []
overview: MinIO secures its APIs with signature-v4, sts, ldap, and oidc across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MinIO
provider_slug: minio
scheme_count: 4
schemes:
- description: Primary S3 data-plane authentication. Requests are signed with AWS Signature Version 4 using an access key ID and secret access key, presented in the Authorization header (or as presigned query parameters). Fully compatible with AWS SDK signing.
  header: Authorization
  location: header
  name: SignatureV4
  scheme: aws-sigv4
  type: signature
- description: Temporary credentials via the MinIO Security Token Service, including AssumeRole, AssumeRoleWithWebIdentity (OIDC), AssumeRoleWithLDAPIdentity, AssumeRoleWithCustomToken, and AssumeRoleWithClientGrants.
  endpoints:
  - AssumeRole
  - AssumeRoleWithWebIdentity
  - AssumeRoleWithLDAPIdentity
  - AssumeRoleWithClientGrants
  - AssumeRoleWithCertificate
  name: STS
  type: sts
- description: External identity via OpenID Connect providers, exchanged for STS credentials.
  name: OIDC
  type: openIdConnect
- description: External identity via LDAP/Active Directory, exchanged for STS credentials.
  name: LDAP
  type: ldap
slug: minio-authentication
source_filename: minio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://min.io/docs/minio/linux/developers/security-token-service.html and https://min.io/docs/minio/linux/administration/identity-access-management.html\nsummary:\n  types: [signature-v4, sts, ldap, oidc]\n  api_key_in: [header]\n  model: access-key/secret-key with AWS Signature Version 4\nschemes:\n- name: SignatureV4\n  type: signature\n  scheme: aws-sigv4\n  description: >-\n    Primary S3 data-plane authentication. Requests are signed with AWS Signature\n    Version 4 using an access key ID and secret access key, presented in the\n    Authorization header (or as presigned query parameters). Fully compatible\n    with AWS SDK signing.\n  location: header\n  header: Authorization\n- name: STS\n  type: sts\n  description: >-\n    Temporary credentials via the MinIO Security Token Service, including\n    AssumeRole, AssumeRoleWithWebIdentity (OIDC), AssumeRoleWithLDAPIdentity,\n    AssumeRoleWithCustomToken, and AssumeRoleWithClientGrants.\n\
  \  endpoints:\n  - AssumeRole\n  - AssumeRoleWithWebIdentity\n  - AssumeRoleWithLDAPIdentity\n  - AssumeRoleWithClientGrants\n  - AssumeRoleWithCertificate\n- name: OIDC\n  type: openIdConnect\n  description: External identity via OpenID Connect providers, exchanged for STS credentials.\n- name: LDAP\n  type: ldap\n  description: External identity via LDAP/Active Directory, exchanged for STS credentials.\npolicies:\n  model: IAM-compatible JSON policies (AWS IAM syntax) attached to users, groups, and service accounts\n  service_accounts: true\nnotes: >-\n  MinIO uses S3/IAM-style key auth, not OAuth scopes; access is governed by\n  IAM-compatible JSON policy documents rather than an OAuth scope registry, so\n  no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/minio/refs/heads/main/authentication/minio-authentication.yml
summary_line: signature-v4/sts/ldap/oidc · 4 schemes
tags:
- Object Storage
- Storage
- S3 Compatible
- Cloud Native
- Kubernetes
- Data Infrastructure
- AI Storage
- Company
---
