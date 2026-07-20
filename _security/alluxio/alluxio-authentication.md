---
api_key_in: []
auth_types:
- http-signature
- none
- tls-mutual
description: ''
kind: authentication
layout: security
method: searched
name: Alluxio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alluxio secures its APIs with http-signature, none, and tls-mutual across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Alluxio
provider_slug: alluxio
scheme_count: 4
schemes:
- description: The S3-compatible REST API parses the AWS Signature V4 Authorization header to extract the username. Under the default SIMPLE mode the signature itself is NOT validated and the secret key may be any non-empty string; if no access key is provided, operations run as the worker process user.
  interface: S3 API
  name: s3-simple-auth
  ports:
    http: 29998
    https: 29996
  scheme: aws-signature-v4
  source: https://documentation.alluxio.io/ee-ai-en/data-access/s3-api.md
  type: http
- description: Alluxio cluster authentication mode; SIMPLE (username from OS) is the default, NOSASL disables auth.
  interface: Alluxio RPC / cluster
  modes:
  - SIMPLE
  - NOSASL
  name: cluster-authentication
  source: https://documentation.alluxio.io/ee-ai-en/administration/security/enabling-authentication.md
  type: sasl
- description: POSIX-style permission model (owner/group/mode) for authorization over Alluxio paths.
  interface: filesystem
  name: authorization
  source: https://documentation.alluxio.io/ee-ai-en/administration/security/enabling-authorization.md
  type: posix-permissions
- description: Optional TLS for securing Alluxio RPC and the S3 API endpoint (HTTPS on port 29996).
  interface: transport
  name: tls
  source: https://documentation.alluxio.io/ee-ai-en/administration/security/securing-alluxio-with-tls.md
  type: mutualTLS
slug: alluxio-authentication
source_filename: alluxio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: >-\n  https://documentation.alluxio.io/ee-ai-en/data-access/s3-api.md ,\n  https://documentation.alluxio.io/ee-ai-en/administration/security/enabling-authentication.md ,\n  https://documentation.alluxio.io/ee-ai-en/administration/security/enabling-authorization.md\nnote: >-\n  Derived from Alluxio docs rather than an OpenAPI spec (Alluxio publishes no OpenAPI). Alluxio is\n  self-hosted, so authentication is a deployment configuration, not a hosted credential issuer.\nsummary:\n  types: [http-signature, none, tls-mutual]\n  interfaces: [s3-api, posix-fuse, python-fsspec]\nschemes:\n  - name: s3-simple-auth\n    interface: S3 API\n    type: http\n    scheme: aws-signature-v4\n    description: >-\n      The S3-compatible REST API parses the AWS Signature V4 Authorization header to extract the\n      username. Under the default SIMPLE mode the signature itself is NOT validated and the secret\n      key may be any non-empty string;\
  \ if no access key is provided, operations run as the worker\n      process user.\n    ports: {http: 29998, https: 29996}\n    source: https://documentation.alluxio.io/ee-ai-en/data-access/s3-api.md\n  - name: cluster-authentication\n    interface: Alluxio RPC / cluster\n    type: sasl\n    modes: [SIMPLE, NOSASL]\n    description: Alluxio cluster authentication mode; SIMPLE (username from OS) is the default, NOSASL disables auth.\n    source: https://documentation.alluxio.io/ee-ai-en/administration/security/enabling-authentication.md\n  - name: authorization\n    interface: filesystem\n    type: posix-permissions\n    description: POSIX-style permission model (owner/group/mode) for authorization over Alluxio paths.\n    source: https://documentation.alluxio.io/ee-ai-en/administration/security/enabling-authorization.md\n  - name: tls\n    interface: transport\n    type: mutualTLS\n    description: Optional TLS for securing Alluxio RPC and the S3 API endpoint (HTTPS on port 29996).\n  \
  \  source: https://documentation.alluxio.io/ee-ai-en/administration/security/securing-alluxio-with-tls.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alluxio/refs/heads/main/authentication/alluxio-authentication.yml
summary_line: http-signature/none/tls-mutual · 4 schemes
tags:
- Company
- Data Orchestration
- Data Caching
- AI Infrastructure
- Machine Learning
- Analytics
- Distributed Storage
- Object Storage
- S3
- Open Source
---
