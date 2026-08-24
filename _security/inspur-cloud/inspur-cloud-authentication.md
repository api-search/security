---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Inspur Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inspur Cloud declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Inspur Cloud
provider_slug: inspur-cloud
scheme_count: 4
schemes:
- applies_to: All platform OpenAPIs (ECS, CPS, EBS, CBS, VPC, EIP, IPTS, SLB, IAM, RDS, TSDB)
  credential: AccessKey ID (AK) + AccessKey Secret (SK), issued by Inspur Cloud IAM
  headers:
  - description: AccessKey ID (AK)
    name: x-secret-id
  - description: Hash algorithm; sha1, md5 and sha256 are supported
    name: x-sign-algorithm
  - description: 13-digit millisecond epoch timestamp
    name: x-time
  - description: Random nonce string, generated per request
    name: x-random
  - description: The computed signature value
    name: x-sign
  id: aksk-signature
  replay_protection: x-time plus x-random act as a timestamp/nonce pair. The docs do not state a clock-skew tolerance or a nonce retention window, so an integrator cannot tell how long a signature stays valid.
  signing_process:
  - detail: Sort all query and form parameters in lexicographic order by key, then join them onto the URI absolute path as uri?key1=value1&key2=value2 to produce uriToSign.
    step: 1
  - detail: Concatenate x-time + x-random + SK, in that order, with no separator, to produce headerToSign.
    step: 2
  - detail: MD5 the request body and hex-encode it to produce bodyToSign.
    step: 3
  - detail: Join httpMethod, headerToSign, uriToSign and bodyToSign with newline separators to produce fullToSign.
    step: 4
  - detail: Hash fullToSign with the chosen algorithm, hex-encode, then base64-encode the result; send it as the x-sign header.
    step: 5
  transport: request headers
  type: custom-signature
  weaknesses:
  - MD5 and SHA-1 are offered as signature algorithms alongside SHA-256, and MD5 is the algorithm used in the worked example in the documentation.
  - The body digest is MD5 regardless of the chosen x-sign-algorithm.
  - The signature is a hash of a concatenated string, not an HMAC; the secret is embedded in the hashed material rather than keying the hash.
- applies_to: Platform OpenAPIs, as an alternative to AK/SK; the Inspur Cloud API Gateway IAM plugin supports both since APIG v1.4.0 (2020-02-27).
  credential: Token obtained from the IAM GetToken interface
  headers:
  - description: Bearer <token>
    name: Authorization
  id: iam-token
  note: The ECS calling-convention page states the Authorization header is required and carries "Bearer [token]" obtained from the GetToken interface. Token lifetime, refresh and revocation are not documented on the public reference pages.
  transport: header
  type: bearer
- algorithm: Signature = base64(HMAC-SHA1(AccessKeySecret, VERB + "\n" + Content-MD5 + "\n" + Content-Type + "\n" + Date + "\n" + CanonicalizedOSSHeaders + CanonicalizedResource))
  applies_to: Object Storage Service (OSS)
  canonical_headers_prefix: x-oss-
  credential: AccessKey ID + AccessKey Secret
  id: oss-signature
  note: This is the Amazon S3 Signature Version 2 construction with an x-oss- header prefix. It is what makes the service usable from S3cmd, S3Browser and Rclone, which Inspur Cloud documents. Invalid signatures return HTTP 403.
  transport: Authorization header, or query-string presigned URL
  type: custom-signature
- applies_to: Inspur Cloud Code Service (ICCS)
  credential: appId + secret issued by the ICCS platform, then a Token
  id: iccs-rsa-signature
  note: Requests are signed with an RSA private key and verified by the platform with the matching public key; a Token obtained from the token endpoint is then sent in the Token header alongside Content-Type application/json.
  transport: Token header
  type: custom-signature
slug: inspur-cloud-authentication
source_filename: inspur-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://console1.cloud.inspur.com/document/iam/9-signate.html\ndocs:\n- https://console1.cloud.inspur.com/document/iam/9-signate.html\n- https://console1.cloud.inspur.com/document/ecs/5-API/5.1-2-invoking-method.html\n- https://console1.cloud.inspur.com/document/oss/5-API/5.3-access-control/01-user-signature.html\nnote: 'Derived by reading the published documentation, not from an OpenAPI securitySchemes\n  block — Inspur Cloud publishes no machine-readable contract. Two distinct signing schemes\n  are in use: a proprietary AK/SK header signature for the platform APIs, and an\n  Amazon-S3-v2-style signature for Object Storage.'\nschemes:\n- id: aksk-signature\n  type: custom-signature\n  applies_to: All platform OpenAPIs (ECS, CPS, EBS, CBS, VPC, EIP, IPTS, SLB, IAM, RDS, TSDB)\n  credential: AccessKey ID (AK) + AccessKey Secret (SK), issued by Inspur Cloud IAM\n  transport: request headers\n  headers:\n  - name: x-secret-id\n\
  \    description: AccessKey ID (AK)\n  - name: x-sign-algorithm\n    description: Hash algorithm; sha1, md5 and sha256 are supported\n  - name: x-time\n    description: 13-digit millisecond epoch timestamp\n  - name: x-random\n    description: Random nonce string, generated per request\n  - name: x-sign\n    description: The computed signature value\n  signing_process:\n  - step: 1\n    detail: 'Sort all query and form parameters in lexicographic order by key, then join them\n      onto the URI absolute path as uri?key1=value1&key2=value2 to produce uriToSign.'\n  - step: 2\n    detail: 'Concatenate x-time + x-random + SK, in that order, with no separator, to produce\n      headerToSign.'\n  - step: 3\n    detail: MD5 the request body and hex-encode it to produce bodyToSign.\n  - step: 4\n    detail: 'Join httpMethod, headerToSign, uriToSign and bodyToSign with newline separators\n      to produce fullToSign.'\n  - step: 5\n    detail: 'Hash fullToSign with the chosen algorithm, hex-encode,\
  \ then base64-encode the\n      result; send it as the x-sign header.'\n  replay_protection: 'x-time plus x-random act as a timestamp/nonce pair. The docs do not\n    state a clock-skew tolerance or a nonce retention window, so an integrator cannot tell\n    how long a signature stays valid.'\n  weaknesses:\n  - 'MD5 and SHA-1 are offered as signature algorithms alongside SHA-256, and MD5 is the\n    algorithm used in the worked example in the documentation.'\n  - 'The body digest is MD5 regardless of the chosen x-sign-algorithm.'\n  - 'The signature is a hash of a concatenated string, not an HMAC; the secret is embedded in\n    the hashed material rather than keying the hash.'\n- id: iam-token\n  type: bearer\n  applies_to: 'Platform OpenAPIs, as an alternative to AK/SK; the Inspur Cloud API Gateway\n    IAM plugin supports both since APIG v1.4.0 (2020-02-27).'\n  credential: Token obtained from the IAM GetToken interface\n  transport: header\n  headers:\n  - name: Authorization\n   \
  \ description: Bearer <token>\n  note: 'The ECS calling-convention page states the Authorization header is required and\n    carries \"Bearer [token]\" obtained from the GetToken interface. Token lifetime, refresh\n    and revocation are not documented on the public reference pages.'\n- id: oss-signature\n  type: custom-signature\n  applies_to: Object Storage Service (OSS)\n  credential: AccessKey ID + AccessKey Secret\n  transport: Authorization header, or query-string presigned URL\n  algorithm: 'Signature = base64(HMAC-SHA1(AccessKeySecret, VERB + \"\\n\" + Content-MD5 + \"\\n\"\n    + Content-Type + \"\\n\" + Date + \"\\n\" + CanonicalizedOSSHeaders + CanonicalizedResource))'\n  canonical_headers_prefix: x-oss-\n  note: 'This is the Amazon S3 Signature Version 2 construction with an x-oss- header prefix.\n    It is what makes the service usable from S3cmd, S3Browser and Rclone, which Inspur Cloud\n    documents. Invalid signatures return HTTP 403.'\n- id: iccs-rsa-signature\n  type:\
  \ custom-signature\n  applies_to: Inspur Cloud Code Service (ICCS)\n  credential: appId + secret issued by the ICCS platform, then a Token\n  transport: Token header\n  note: 'Requests are signed with an RSA private key and verified by the platform with the\n    matching public key; a Token obtained from the token endpoint is then sent in the Token\n    header alongside Content-Type application/json.'\noauth2: false\nopenid_connect: false\nmutual_tls: false\nmfa:\n  supported: true\n  detail: 'IAM exposes TOTP MFA management operations — GET /auth/v1/users/{userId}/action/\n    get-totp-register-info, POST .../bind-totp, PUT .../remove-totp, GET .../has-totp — so\n    MFA is an account control, not an API authentication factor.'\ngaps:\n- No OAuth 2.0 or OpenID Connect surface is published anywhere in the documentation.\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server document\n  is served on any host (see well-known/inspur-cloud-well-known.yml).\n- 'Token\
  \ lifetime, rotation and revocation are undocumented, as is the signature validity\n  window; an integrator has to discover both empirically.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inspur-cloud/refs/heads/main/authentication/inspur-cloud-authentication.yml
summary_line: 4 schemes
tags:
- Cloud
- Infrastructure
- Compute
- Storage
- Networking
- Object Storage
- Identity
- Database
- Containers
- Internet of Things
- Blockchain
- China
- Company
---
