---
api_key_in: []
api_specs:
- filename: logicmonitor-rest-api-v3-swagger.json
  format: json
  label: LogicMonitor REST API v3
  slug: logicmonitor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicmonitor/refs/heads/main/openapi/logicmonitor-rest-api-v3-swagger.json
auth_types: []
description: 'LogicMonitor REST API authentication. The published v3 Swagger declares exactly one security scheme — an apiKey named LMv1 carried in the Authorization header — and applies it per operation rather than globally. The docs add two further methods the contract does not model: a Bearer token (the recommended method for v3 and for the Python and Go SDKs) and HTTP Basic, which is v1-only and explicitly discouraged. There is no OAuth 2.0, no OpenID Connect and no mutual TLS on this API.'
kind: authentication
layout: security
method: searched
name: Logicmonitor Authentication
name_suffix: Authentication
oauth_flows: []
overview: LogicMonitor declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: LogicMonitor
provider_slug: logicmonitor
scheme_count: 3
schemes:
- clock_skew: request timestamp must be within 30 minutes of server time
  declared_in_spec: true
  format: 'Authorization: LMv1 AccessId:Signature:Timestamp'
  id: LMv1
  in: header
  name: Authorization
  note: Query parameters (filter, fields, sort, size) are NOT part of the resource path and must be excluded from the signature calculation. Permissions are those of the API token's role.
  signing: HMAC-SHA256, base64-encoded
  signing_string: HTTP_VERB + TIMESTAMP_EPOCH_MS + POST_OR_PUT_BODY + RESOURCE_PATH
  type: apiKey
- declared_in_spec: false
  id: Bearer
  in: header
  name: Authorization
  note: Auto-generated per user, unique per user, no specific role required to obtain one. Recommended for REST API v3 and required by the documented Python and Go v3 SDKs (configuration.auth_type = 'Bearer' / config.SetBearerToken()). Partially masked with asterisks once saved in the portal.
  scheme: bearer
  type: http
- declared_in_spec: false
  deprecated: true
  id: Basic
  in: header
  name: Authorization
  note: Supported only by REST API v1. The docs say it "may not be available with future versions of the API" and recommend token-based authentication instead.
  scheme: basic
  type: http
slug: logicmonitor-authentication
source_filename: logicmonitor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: LogicMonitor\nproviderId: logicmonitor\ngenerated: '2026-08-29'\nmethod: searched\nsource: https://www.logicmonitor.com/support/rest-api-authentication\ndocs: https://www.logicmonitor.com/support/rest-api-authentication\nspec: openapi/logicmonitor-rest-api-v3-swagger.json\ndescription: >-\n  LogicMonitor REST API authentication. The published v3 Swagger declares exactly one security scheme —\n  an apiKey named LMv1 carried in the Authorization header — and applies it per operation rather than\n  globally. The docs add two further methods the contract does not model: a Bearer token (the recommended\n  method for v3 and for the Python and Go SDKs) and HTTP Basic, which is v1-only and explicitly discouraged.\n  There is no OAuth 2.0, no OpenID Connect and no mutual TLS on this API.\nschemes:\n  - id: LMv1\n    type: apiKey\n    in: header\n    name: Authorization\n    declared_in_spec: true\n   \
  \ format: 'Authorization: LMv1 AccessId:Signature:Timestamp'\n    signing: HMAC-SHA256, base64-encoded\n    signing_string: HTTP_VERB + TIMESTAMP_EPOCH_MS + POST_OR_PUT_BODY + RESOURCE_PATH\n    clock_skew: request timestamp must be within 30 minutes of server time\n    note: >-\n      Query parameters (filter, fields, sort, size) are NOT part of the resource path and must be excluded\n      from the signature calculation. Permissions are those of the API token's role.\n  - id: Bearer\n    type: http\n    scheme: bearer\n    in: header\n    name: Authorization\n    declared_in_spec: false\n    note: >-\n      Auto-generated per user, unique per user, no specific role required to obtain one. Recommended for\n      REST API v3 and required by the documented Python and Go v3 SDKs (configuration.auth_type = 'Bearer' /\n      config.SetBearerToken()). Partially masked with asterisks once saved in the portal.\n  - id: Basic\n    type: http\n    scheme: basic\n    in: header\n    name: Authorization\n\
  \    declared_in_spec: false\n    deprecated: true\n    note: >-\n      Supported only by REST API v1. The docs say it \"may not be available with future versions of the API\"\n      and recommend token-based authentication instead.\noauth2: false\nopenid_connect: false\nmutual_tls: false\ntransport: HTTPS required on every request\nidentity_federation:\n  sso:\n    - SAML 2.0\n    - Microsoft Entra ID (Azure Active Directory)\n    - Okta\n  scim: true\n  scim_note: >-\n    SCIM is supported for user lifecycle synchronization and de-provisioning from an IdP, gated on a\n    Manage permission for Single Sign-On. See conformance/logicmonitor-conformance.yml.\n  mfa: Two-factor authentication and passkeys are available on portal accounts; error 1412/HTTP 412 signals an unmet 2FA precondition.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logicmonitor/refs/heads/main/authentication/logicmonitor-authentication.yml
summary_line: 3 schemes
tags:
- AIOps
- Monitoring
- Observability
- Infrastructure
- Log Management
- Network Monitoring
- Cloud Monitoring
- Alerting
- Synthetic Monitoring
- OpenTelemetry
- ITOps
---
