---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-lightsail-openapi.yml
  format: yaml
  label: Amazon Lightsail API
  slug: amazon-lightsail-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-lightsail/refs/heads/main/openapi/amazon-lightsail-openapi.yml
auth_types:
- sigv4
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Amazon Lightsail Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Lightsail secures its APIs with sigv4 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Lightsail
provider_slug: amazon-lightsail
scheme_count: 1
schemes:
- algorithm: AWS4-HMAC-SHA256
  description: Sign each request with AWS Signature Version 4. The Authorization header carries the credential scope (access key / date / region / service / aws4_request), the signed header list and the signature. Requests may alternatively carry the signature in query-string form using X-Amz-Algorithm, X-Amz-Credential, X-Amz-Date, X-Amz-SignedHeaders and X-Amz-Signature.
  in: header
  name: sigv4
  parameter: Authorization
  service_name: lightsail
  sources:
  - smithy/amazon-lightsail-2016-11-28.json
  - openapi/amazon-lightsail-openapi.yml
  - https://docs.aws.amazon.com/lightsail/2016-11-28/api-reference/CommonParameters.html
  temporary_credentials:
    header: X-Amz-Security-Token
    note: Required when signing with temporary credentials from AWS STS (assumed roles, SSO, instance profiles).
    supported: true
  type: sigv4
slug: amazon-lightsail-authentication
source_filename: amazon-lightsail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: >-\n  https://docs.aws.amazon.com/lightsail/2016-11-28/api-reference/CommonParameters.html (fetched\n  2026-09-17, HTTP 200) and the aws.auth#sigv4 trait in smithy/amazon-lightsail-2016-11-28.json,\n  rendered into openapi/amazon-lightsail-openapi.yml.\ndocs: https://docs.aws.amazon.com/lightsail/2016-11-28/api-reference/CommonParameters.html\nprovider: Amazon Lightsail\nproviderId: amazon-lightsail\nsummary:\n  types:\n  - sigv4\n  api_key_in:\n  - header\n  oauth: false\n  openid_connect: false\n  mutual_tls: false\nnote: >-\n  Lightsail has exactly one authentication mechanism and no alternative: AWS Signature Version 4 over\n  IAM credentials, with service name \"lightsail\". There is no API key you can paste into a header, no\n  OAuth flow, no personal access token, and no scope surface — authorization is expressed entirely as\n  IAM policy on lightsail:* actions, which is why scopes/ is deliberately absent from this repository\n\
  \  rather than empty. The practical consequence for an agent is that credentials cannot be delegated\n  per-call: whatever IAM principal signs the request carries its full policy, so least privilege has to\n  be arranged in advance by issuing a narrowly-scoped role, not negotiated at call time. Every call is\n  recorded in CloudTrail under the event source lightsail.amazonaws.com.\nschemes:\n- name: sigv4\n  type: sigv4\n  in: header\n  parameter: Authorization\n  algorithm: AWS4-HMAC-SHA256\n  service_name: lightsail\n  description: >-\n    Sign each request with AWS Signature Version 4. The Authorization header carries the credential\n    scope (access key / date / region / service / aws4_request), the signed header list and the\n    signature. Requests may alternatively carry the signature in query-string form using X-Amz-Algorithm,\n    X-Amz-Credential, X-Amz-Date, X-Amz-SignedHeaders and X-Amz-Signature.\n  temporary_credentials:\n    supported: true\n    header: X-Amz-Security-Token\n\
  \    note: Required when signing with temporary credentials from AWS STS (assumed roles, SSO, instance profiles).\n  sources:\n  - smithy/amazon-lightsail-2016-11-28.json\n  - openapi/amazon-lightsail-openapi.yml\n  - https://docs.aws.amazon.com/lightsail/2016-11-28/api-reference/CommonParameters.html\nauthorization:\n  model: AWS IAM policy\n  actions_prefix: 'lightsail:'\n  scopes_published: false\n  note: >-\n    Permissions are IAM actions (lightsail:GetInstances, lightsail:CreateInstances, ...), one per API\n    operation, attachable to users and roles and constrainable by resource ARN and condition keys.\n    There is no OAuth scope document to enumerate.\n  audit: CloudTrail, event source lightsail.amazonaws.com\nfailure_modes:\n- exception: UnauthenticatedException\n  status: 401\n  cause: Request was not signed, or the signature could not be validated.\n- exception: AccessDeniedException\n  status: 403\n  cause: Signed correctly but the IAM principal's policy does not allow the\
  \ action.\n- exception: ExpiredTokenException\n  status: 403\n  cause: Temporary STS credentials expired. Re-assume the role.\n- exception: IncompleteSignature\n  status: 403\n  cause: Malformed SigV4 signature — usually a clock skew or a canonical-request mistake.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-lightsail/refs/heads/main/authentication/amazon-lightsail-authentication.yml
summary_line: sigv4 · 1 scheme
tags:
- Cloud
- Compute
- Virtual Private Server
- Hosting
- Containers
- Database
- Storage
- CDN
- Networking
- Infrastructure
- DevOps
---
