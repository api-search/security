---
api_key_in:
- query
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Infutor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Infutor secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Infutor
provider_slug: infutor
scheme_count: 5
schemes:
- example: https://api.leadid.com/Authenticate?lac={ACCOUNTCODE}&id={LEADIDTOKEN}
  in: query
  name: leadidQueryCredentials
  parameters:
  - description: Account Code (UUID) issued by InfutorData / LeadiD.
    name: lac
    required: true
  - description: LeadiD token to authenticate/audit (UUID); may be optional when "LeadiD Optional" is enabled.
    name: id
    required: false
  source: https://help.infutor.com/apidocs/endpoint-for-a-lead-audit.md
  type: apiKey
- description: Optional Bearer token in the Authorization header, required when API Authentication is enabled on the LeadiD query endpoints (e.g. /SingleQuery).
  header: Authorization
  in: header
  name: bearerToken
  scheme: bearer
  source: https://help.infutor.com/apidocs/endpoint-for-a-lead-audit.md
  type: http
- description: The Audit / Intelligence API requires a customer-supplied `authorization` request header carrying the token(s) InfutorData generates for the account.
  header: authorization
  in: header
  name: audit_authorization_token
  source: https://help.infutor.com/docs/infutor-api.md
  type: apiKey
- applies_to:
  - GET https://app.jornaya.com/api/v1/activate
  - GET https://app.jornaya.com/api/v1/activate/{activate_instance_id}/upload
  - GET https://app.jornaya.com/api/v1/activate/{activate_instance_id}/runs
  - GET https://app.jornaya.com/api/v1/activate/{activate_instance_id}/runs/{run_date}
  description: 'API Access Token for the batch Activate API, minted by the customer in myJornaya at https://app.jornaya.com/activate/access-tokens ("Add API Token") and sent as `Authorization: Bearer <token>`. Deleting a token immediately breaks any process using it; there is no rotation window, grace period or expiry documented.'
  header: Authorization
  in: header
  management_url: https://app.jornaya.com/activate/access-tokens
  name: activateAccessToken
  scheme: bearer
  self_service: true
  source: https://help.infutor.com/docs/api-endpoint-monitoring-file-send.md
  type: http
  verification:
    body: '{"Code":"UnauthorizedQuery","Message":"Missing Authorization Token"}'
    http_status: 401
    method: probed
    request: GET https://app.jornaya.com/api/v1/activate (no Authorization header)
- description: 'The monitoring-file upload is a presigned S3 form POST. The GET /upload call returns the URL plus the form-data fields the client must replay: key, x-amz-algorithm, x-amz-credential, x-amz-date, x-amz-security-token, policy and x-amz-signature. These are short-lived AWS credentials scoped to one upload, not an InfutorData API credential.'
  in: body
  name: activateUploadSignature
  source: https://help.infutor.com/docs/api-endpoint-monitoring-file-send.md
  type: aws-sigv4-presigned-post
slug: infutor-authentication
source_filename: infutor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.infutor.com/docs/authentication-api.md\ndocs: https://help.infutor.com/docs/infutor-api.md\nsummary:\n  types: [apiKey, http]\n  api_key_in: [query, header]\n  oauth2_flows: []\n  notes: >-\n    InfutorData / LeadiD (part of ActiveProspect) uses account-code + LeadiD-token\n    query-parameter credentials on the LeadiD query APIs, plus an optional HTTP\n    Bearer token in the Authorization header when API Authentication is enabled.\n    The Audit/Intelligence API additionally documents a customer-supplied\n    `authorization: {token}` request header carrying InfutorData-generated tokens.\n    The separate batch Activate API on app.jornaya.com uses a self-service\n    Bearer API access token minted in myJornaya, and its presigned upload step\n    uses AWS SigV4 form fields rather than an InfutorData credential.\n  provisioning: >-\n    Credentials for the LeadiD query APIs are issued by InfutorData support, not\n\
  \    self-service — the account code, audit profile key and (where enabled) the\n    authentication token all come from customersupport@infutor.com. Only the\n    Activate API access token can be created by the customer.\nschemes:\n  - name: leadidQueryCredentials\n    type: apiKey\n    in: query\n    parameters:\n      - name: lac\n        description: Account Code (UUID) issued by InfutorData / LeadiD.\n        required: true\n      - name: id\n        description: LeadiD token to authenticate/audit (UUID); may be optional when \"LeadiD Optional\" is enabled.\n        required: false\n    source: https://help.infutor.com/apidocs/endpoint-for-a-lead-audit.md\n    example: https://api.leadid.com/Authenticate?lac={ACCOUNTCODE}&id={LEADIDTOKEN}\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    description: >-\n      Optional Bearer token in the Authorization header, required when API\n      Authentication is enabled on the LeadiD query\
  \ endpoints (e.g. /SingleQuery).\n    source: https://help.infutor.com/apidocs/endpoint-for-a-lead-audit.md\n  - name: audit_authorization_token\n    type: apiKey\n    in: header\n    header: authorization\n    description: >-\n      The Audit / Intelligence API requires a customer-supplied `authorization`\n      request header carrying the token(s) InfutorData generates for the account.\n    source: https://help.infutor.com/docs/infutor-api.md\n  - name: activateAccessToken\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    applies_to:\n      - 'GET https://app.jornaya.com/api/v1/activate'\n      - 'GET https://app.jornaya.com/api/v1/activate/{activate_instance_id}/upload'\n      - 'GET https://app.jornaya.com/api/v1/activate/{activate_instance_id}/runs'\n      - 'GET https://app.jornaya.com/api/v1/activate/{activate_instance_id}/runs/{run_date}'\n    description: >-\n      API Access Token for the batch Activate API, minted by the customer in\n      myJornaya\
  \ at https://app.jornaya.com/activate/access-tokens (\"Add API\n      Token\") and sent as `Authorization: Bearer <token>`. Deleting a token\n      immediately breaks any process using it; there is no rotation window,\n      grace period or expiry documented.\n    self_service: true\n    management_url: https://app.jornaya.com/activate/access-tokens\n    source: https://help.infutor.com/docs/api-endpoint-monitoring-file-send.md\n    verification:\n      method: probed\n      request: 'GET https://app.jornaya.com/api/v1/activate (no Authorization header)'\n      http_status: 401\n      body: '{\"Code\":\"UnauthorizedQuery\",\"Message\":\"Missing Authorization Token\"}'\n  - name: activateUploadSignature\n    type: aws-sigv4-presigned-post\n    in: body\n    description: >-\n      The monitoring-file upload is a presigned S3 form POST. The GET\n      /upload call returns the URL plus the form-data fields the client must\n      replay: key, x-amz-algorithm, x-amz-credential, x-amz-date,\n\
  \      x-amz-security-token, policy and x-amz-signature. These are short-lived\n      AWS credentials scoped to one upload, not an InfutorData API credential.\n    source: https://help.infutor.com/docs/api-endpoint-monitoring-file-send.md\ntransport_security:\n  tls_minimum: TLS 1.2\n  cipher_suites_published: true\n  source: https://help.infutor.com/docs/authentication-api.md\n  note: >-\n    17 supported cipher suites are enumerated verbatim in the API articles, with\n    a commitment to notify customers in advance of any revision.\ndiscovery_probes:\n  note: >-\n    No OAuth 2.0 or OpenID Connect metadata is served on any host; there is no\n    scope surface, so no scopes/ artifact is emitted.\n  probes:\n    - url: https://api.leadid.com/.well-known/openid-configuration\n      status: 404\n    - url: https://api.leadid.com/.well-known/oauth-authorization-server\n      status: 404\n    - url: https://help.infutor.com/.well-known/oauth-authorization-server\n      status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infutor/refs/heads/main/authentication/infutor-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Company
- Identity Resolution
- Consumer Data
- Data Enrichment
- Lead Verification
- TCPA Compliance
- Marketing
- Identity
---
