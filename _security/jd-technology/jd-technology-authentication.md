---
api_key_in:
- header
auth_types:
- requestSignature
description: ''
kind: authentication
layout: security
method: searched
name: Jd Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: JD Technology secures its APIs with requestSignature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: JD Technology
provider_slug: jd-technology
scheme_count: 2
schemes:
- credential_source: JD Cloud console (access-key / secret-key)
  description: Requests to <service>.jdcloud-api.com are signed with an access-key (AK) and secret-key (SK) pair issued from the JD Cloud console. The client computes an HMAC signature over the canonical request and passes it, together with the access key and timestamp, in request headers. Dedicated per-language signer utilities (jdcloud-sdk-*-signer) implement the algorithm; the SDKs and jdc CLI sign automatically.
  name: JDCloudSignature
  signers:
  - https://github.com/jdcloud-api/jdcloud-sdk-java-signer
  - https://github.com/jdcloud-api/jdcloud-sdk-go-signer
  - https://github.com/jdcloud-api/jdcloud-sdk-nodejs-signer
  - https://github.com/jdcloud-api/jdcloud-sdk-net-signer
  - https://github.com/jdcloud-api/jdcloud-sdk-php-signer
  - https://github.com/jdcloud-api/jdcloud-sdk-cpp-signer
  - https://github.com/jdcloud-api/jdcloud-sdk-rust-signer
  type: requestSignature
- description: MFA / operation-protection token required when calling operations protected by multi-factor operation protection. Passed as an additional header alongside the request signature.
  in: header
  name: MFAOperationToken
  parameter: x-jdcloud-security-token
  type: apiKey
slug: jd-technology-authentication
source_filename: jd-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.jdcloud.com/cn/common-declaration/api/introduction\nnotes: >-\n  JD Cloud OpenAPI is not documented via an OpenAPI securityScheme in this repo\n  (no spec harvested yet); this profile is captured from the JD Cloud OpenAPI\n  documentation and CLI. JD Cloud uses an AWS-style request-signature scheme\n  rather than a bearer token or OAuth.\nsummary:\n  types:\n  - requestSignature\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: JDCloudSignature\n  type: requestSignature\n  description: >-\n    Requests to <service>.jdcloud-api.com are signed with an access-key (AK) and\n    secret-key (SK) pair issued from the JD Cloud console. The client computes an\n    HMAC signature over the canonical request and passes it, together with the\n    access key and timestamp, in request headers. Dedicated per-language signer\n    utilities (jdcloud-sdk-*-signer) implement the algorithm; the SDKs and jdc CLI\n  \
  \  sign automatically.\n  credential_source: JD Cloud console (access-key / secret-key)\n  signers:\n  - https://github.com/jdcloud-api/jdcloud-sdk-java-signer\n  - https://github.com/jdcloud-api/jdcloud-sdk-go-signer\n  - https://github.com/jdcloud-api/jdcloud-sdk-nodejs-signer\n  - https://github.com/jdcloud-api/jdcloud-sdk-net-signer\n  - https://github.com/jdcloud-api/jdcloud-sdk-php-signer\n  - https://github.com/jdcloud-api/jdcloud-sdk-cpp-signer\n  - https://github.com/jdcloud-api/jdcloud-sdk-rust-signer\n- name: MFAOperationToken\n  type: apiKey\n  in: header\n  parameter: x-jdcloud-security-token\n  description: >-\n    MFA / operation-protection token required when calling operations protected by\n    multi-factor operation protection. Passed as an additional header alongside the\n    request signature.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jd-technology/refs/heads/main/authentication/jd-technology-authentication.yml
summary_line: requestSignature · 2 schemes
tags:
- Company
- Technology
- Cloud
- Cloud Computing
- Infrastructure
- Fintech
- Artificial Intelligence
- Developer Platform
- OpenAPI
- China
---
