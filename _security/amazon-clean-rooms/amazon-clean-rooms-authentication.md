---
api_key_in:
- header
api_specs:
- filename: amazon-clean-rooms-collaborations-api-openapi.yml
  format: yaml
  label: Amazon Clean Rooms Collaborations API
  slug: amazon-clean-rooms-collaborations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/openapi/amazon-clean-rooms-collaborations-api-openapi.yml
- filename: amazon-clean-rooms-configured-tables-api-openapi.yml
  format: yaml
  label: Amazon Clean Rooms Configured Tables API
  slug: amazon-clean-rooms-configured-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/openapi/amazon-clean-rooms-configured-tables-api-openapi.yml
- filename: amazon-clean-rooms-memberships-api-openapi.yml
  format: yaml
  label: Amazon Clean Rooms Memberships API
  slug: amazon-clean-rooms-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/openapi/amazon-clean-rooms-memberships-api-openapi.yml
- filename: amazon-clean-rooms-protected-queries-api-openapi.yml
  format: yaml
  label: Amazon Clean Rooms Protected Queries API
  slug: amazon-clean-rooms-protected-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/openapi/amazon-clean-rooms-protected-queries-api-openapi.yml
auth_types:
- aws-sigv4
description: ''
kind: authentication
layout: security
method: searched
name: Amazon Clean Rooms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Clean Rooms secures its APIs with aws-sigv4 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Clean Rooms
provider_slug: amazon-clean-rooms
scheme_count: 1
schemes:
- algorithm: AWS4-HMAC-SHA256
  description: AWS Signature Version 4. The Authorization header carries the credential scope (access key / date / region / service / aws4_request), the signed header list, and the hex signature.
  in: header
  name: aws_signature
  parameter: Authorization
  region_scoped: true
  service_name: cleanrooms
  sources:
  - openapi/amazon-clean-rooms-collaborations-api-openapi.yml
  - openapi/amazon-clean-rooms-configured-tables-api-openapi.yml
  - openapi/amazon-clean-rooms-memberships-api-openapi.yml
  - openapi/amazon-clean-rooms-protected-queries-api-openapi.yml
  - https://docs.aws.amazon.com/clean-rooms/latest/apireference/CommonParameters.html
  spec_type: apiKey
  type: aws-sigv4
slug: amazon-clean-rooms-authentication
source_filename: amazon-clean-rooms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://docs.aws.amazon.com/clean-rooms/latest/apireference/CommonParameters.html\n  and https://docs.aws.amazon.com/clean-rooms/latest/userguide/security-iam.html,\n  reconciled against the securitySchemes derived from openapi/*.yml.\ndocs: https://docs.aws.amazon.com/clean-rooms/latest/apireference/CommonParameters.html\nsummary:\n  types:\n  - aws-sigv4\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    The captured OpenAPI models AWS SigV4 as an apiKey-in-header scheme because\n    OpenAPI 3.1 has no native SigV4 type. That is a spec-shape artifact, not the\n    real model: SigV4 is a request-signing scheme over the whole canonical\n    request, not a static key placed in a header. Recorded here as aws-sigv4 so\n    downstream consumers are not told to paste a bearer token.\nschemes:\n- name: aws_signature\n  type: aws-sigv4\n  spec_type: apiKey\n  in: header\n\
  \  parameter: Authorization\n  algorithm: AWS4-HMAC-SHA256\n  service_name: cleanrooms\n  region_scoped: true\n  description: >-\n    AWS Signature Version 4. The Authorization header carries the credential\n    scope (access key / date / region / service / aws4_request), the signed\n    header list, and the hex signature.\n  sources:\n  - openapi/amazon-clean-rooms-collaborations-api-openapi.yml\n  - openapi/amazon-clean-rooms-configured-tables-api-openapi.yml\n  - openapi/amazon-clean-rooms-memberships-api-openapi.yml\n  - openapi/amazon-clean-rooms-protected-queries-api-openapi.yml\n  - https://docs.aws.amazon.com/clean-rooms/latest/apireference/CommonParameters.html\nquery_string_signing:\n  supported: true\n  note: >-\n    Authentication information may be placed in the query string instead of the\n    Authorization header (presigned-style), using the parameters below.\n  parameters:\n  - name: X-Amz-Algorithm\n    values: [AWS4-HMAC-SHA256]\n    required: conditional\n  - name: X-Amz-Credential\n\
  \    format: access_key/YYYYMMDD/region/service/aws4_request\n    required: conditional\n  - name: X-Amz-Date\n    format: ISO 8601 basic (YYYYMMDD'T'HHMMSS'Z')\n    required: conditional\n  - name: X-Amz-Signature\n    required: conditional\n  - name: X-Amz-SignedHeaders\n    required: conditional\n  - name: X-Amz-Security-Token\n    required: conditional\n    note: Required when using temporary credentials from AWS STS.\ntemporary_credentials:\n  supported: true\n  issuer: AWS Security Token Service (STS)\n  header: X-Amz-Security-Token\nauthorization:\n  model: AWS IAM + collaboration member abilities\n  action_namespace: cleanrooms:*\n  managed_policies:\n  - AWSCleanRoomsFullAccess\n  - AWSCleanRoomsFullAccessNoQuerying\n  - AWSCleanRoomsReadOnlyAccess\n  - AWSCleanRoomsMLFullAccess\n  - AWSCleanRoomsMLReadOnlyAccess\n  member_abilities:\n  - CAN_QUERY\n  - CAN_RECEIVE_RESULTS\n  - CAN_RUN_JOB\n  - CAN_EXPORT_QUERY_ANALYSIS_LOG\n  note: >-\n    Two independent authorization layers.\
  \ IAM decides whether the calling\n    principal may invoke the API at all; the collaboration's member abilities\n    decide what that member may do inside a given collaboration. A principal with\n    full IAM access still cannot query if its membership lacks CAN_QUERY.\n  docs: https://docs.aws.amazon.com/clean-rooms/latest/userguide/security-iam.html\n  service_roles: https://docs.aws.amazon.com/clean-rooms/latest/userguide/setting-up-roles.html\nscopes:\n  applicable: false\n  note: >-\n    No OAuth 2.0 surface, therefore no scope registry. Access is expressed as IAM\n    actions and member abilities, not scopes — scopes/ is intentionally absent\n    rather than empty.\nerrors:\n- code: IncompleteSignature\n  status: 403\n- code: UnrecognizedClientException\n  status: 403\n- code: ExpiredTokenException\n  status: 403\n- code: AccessDeniedException\n  status: 403\n- code: NotAuthorized\n  status: 401\ncatalog: errors/amazon-clean-rooms-error-codes.yml\nconventions: conventions/amazon-clean-rooms-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/authentication/amazon-clean-rooms-authentication.yml
summary_line: aws-sigv4 · 1 scheme
tags:
- Clean Rooms
- Data Collaboration
- Privacy
- Analytics
- Marketing
---
