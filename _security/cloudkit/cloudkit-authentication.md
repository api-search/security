---
anonymous_access: false
api_key_in:
- query
- header
api_specs:
- filename: cloudkit-assets-api-openapi.yml
  format: yaml
  label: Apple CloudKit Assets API
  slug: cloudkit-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/openapi/cloudkit-assets-api-openapi.yml
- filename: cloudkit-changes-api-openapi.yml
  format: yaml
  label: Apple CloudKit Changes API
  slug: cloudkit-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/openapi/cloudkit-changes-api-openapi.yml
- filename: cloudkit-records-api-openapi.yml
  format: yaml
  label: Apple CloudKit Records API
  slug: cloudkit-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/openapi/cloudkit-records-api-openapi.yml
- filename: cloudkit-subscriptions-api-openapi.yml
  format: yaml
  label: Apple CloudKit Subscriptions API
  slug: cloudkit-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/openapi/cloudkit-subscriptions-api-openapi.yml
- filename: cloudkit-tokens-api-openapi.yml
  format: yaml
  label: Apple CloudKit Tokens API
  slug: cloudkit-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/openapi/cloudkit-tokens-api-openapi.yml
- filename: cloudkit-users-api-openapi.yml
  format: yaml
  label: Apple CloudKit Users API
  slug: cloudkit-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/openapi/cloudkit-users-api-openapi.yml
- filename: cloudkit-zones-api-openapi.yml
  format: yaml
  label: Apple CloudKit Zones API
  slug: cloudkit-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/openapi/cloudkit-zones-api-openapi.yml
auth_types:
- apiKey
- signature
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Cloudkit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apple CloudKit secures its APIs with apiKey and signature across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Apple CloudKit
provider_slug: cloudkit
scheme_count: 4
schemes:
- description: CloudKit API token created in the CloudKit Console and appended to the request URL as `?ckAPIToken=[API token]`. Identifies the app; on its own it grants only what the public database allows to an unauthenticated caller.
  in: query
  issued_from: CloudKit Console (per container)
  name: cloudKitApiToken
  parameter: ckAPIToken
  sources:
  - https://developer.apple.com/library/archive/documentation/DataManagement/Conceptual/CloudKitWebServicesReference/SettingUpWebServices.html
  type: apiKey
- description: End-user session token appended alongside ckAPIToken. Obtained by making the request without it, receiving AUTHENTICATION_REQUIRED (HTTP 421) with a `redirectURL`, opening that URL so Apple can present its own sign-in dialog, and reading the token back from the callback (URL parameter or a `message` event carrying `e.data.ckWebAuthToken`). Must be URL-encoded when appended — Apple calls out replacing `+` with `%2B`, `/` with `%2F` and `=` with `%3D`.
  in: query
  lifetime: Default expiration 30 minutes after creation; two weeks if the user selects "Keep me signed in". Each token is for a single round trip.
  name: ckWebAuthToken
  parameter: ckWebAuthToken
  sources:
  - https://developer.apple.com/library/archive/documentation/DataManagement/Conceptual/CloudKitWebServicesReference/SettingUpWebServices.html
  type: apiKey
- constraints:
  - Signed requests expire 10 minutes after their ISO8601 date; server clock accuracy matters.
  - Do NOT include the ckAPIToken subpath in a server-to-server request — Apple states it will fail.
  - Do NOT mix API-token and server-to-server authentication in the same request.
  description: Server-to-server access signs each request with an ECDSA (prime256v1) private key whose public half was uploaded to the CloudKit Console in exchange for a Key ID. The signed message is `[ISO8601 date]:[base64 SHA-256 of the request body]:[URL subpath]`.
  headers:
  - X-Apple-CloudKit-Request-KeyID
  - X-Apple-CloudKit-Request-ISO8601Date
  - X-Apple-CloudKit-Request-SignatureV1
  in: header
  key_generation: openssl ecparam -name prime256v1 -genkey -noout -out eckey.pem
  name: serverToServer
  parameter: X-Apple-CloudKit-Request-SignatureV1
  sources:
  - https://developer.apple.com/library/archive/documentation/DataManagement/Conceptual/CloudKitWebServicesReference/SettingUpWebServices.html
  type: apiKey
- description: Generated in the CloudKit Console under Settings for your user account and shown only once. cktool stores management and user tokens in the macOS Keychain via `xcrun cktool save-token`.
  in: header
  name: managementToken
  parameter: null
  scope: CloudKit Management API (schema operations via cktool / CKTool JS), not the database API
  sources:
  - https://developer.apple.com/icloud/ck-tool/
  type: apiKey
slug: cloudkit-authentication
source_filename: cloudkit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://developer.apple.com/library/archive/documentation/DataManagement/Conceptual/CloudKitWebServicesReference/SettingUpWebServices.html,\n  https://developer.apple.com/documentation/cloudkit/obtaining-an-api-token-for-an-icloud-container,\n  https://developer.apple.com/icloud/ck-tool/, openapi/_original/cloudkit-openapi.yml\ndocs: https://developer.apple.com/library/archive/documentation/DataManagement/Conceptual/CloudKitWebServicesReference/SettingUpWebServices.html\nsummary:\n  types:\n  - apiKey\n  - signature\n  api_key_in:\n  - query\n  - header\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  note: >-\n    Three distinct credentials, and Apple states two of them MUST NOT be combined in one request: an API\n    token (+ optional user web-auth token) for user-facing access, an ECDSA server-to-server key for\n    backend access, and a management token used only by cktool / CKTool JS against the CloudKit\n\
  \    Management API.\nschemes:\n- name: cloudKitApiToken\n  type: apiKey\n  in: query\n  parameter: ckAPIToken\n  issued_from: CloudKit Console (per container)\n  description: >-\n    CloudKit API token created in the CloudKit Console and appended to the request URL as\n    `?ckAPIToken=[API token]`. Identifies the app; on its own it grants only what the public database\n    allows to an unauthenticated caller.\n  sources:\n  - https://developer.apple.com/library/archive/documentation/DataManagement/Conceptual/CloudKitWebServicesReference/SettingUpWebServices.html\n- name: ckWebAuthToken\n  type: apiKey\n  in: query\n  parameter: ckWebAuthToken\n  description: >-\n    End-user session token appended alongside ckAPIToken. Obtained by making the request without it,\n    receiving AUTHENTICATION_REQUIRED (HTTP 421) with a `redirectURL`, opening that URL so Apple can\n    present its own sign-in dialog, and reading the token back from the callback (URL parameter or a\n    `message` event carrying\
  \ `e.data.ckWebAuthToken`). Must be URL-encoded when appended — Apple calls\n    out replacing `+` with `%2B`, `/` with `%2F` and `=` with `%3D`.\n  lifetime: >-\n    Default expiration 30 minutes after creation; two weeks if the user selects \"Keep me signed in\".\n    Each token is for a single round trip.\n  sources:\n  - https://developer.apple.com/library/archive/documentation/DataManagement/Conceptual/CloudKitWebServicesReference/SettingUpWebServices.html\n- name: serverToServer\n  type: apiKey\n  in: header\n  parameter: X-Apple-CloudKit-Request-SignatureV1\n  description: >-\n    Server-to-server access signs each request with an ECDSA (prime256v1) private key whose public half\n    was uploaded to the CloudKit Console in exchange for a Key ID. The signed message is\n    `[ISO8601 date]:[base64 SHA-256 of the request body]:[URL subpath]`.\n  headers:\n  - X-Apple-CloudKit-Request-KeyID\n  - X-Apple-CloudKit-Request-ISO8601Date\n  - X-Apple-CloudKit-Request-SignatureV1\n  key_generation:\
  \ openssl ecparam -name prime256v1 -genkey -noout -out eckey.pem\n  constraints:\n  - Signed requests expire 10 minutes after their ISO8601 date; server clock accuracy matters.\n  - Do NOT include the ckAPIToken subpath in a server-to-server request — Apple states it will fail.\n  - Do NOT mix API-token and server-to-server authentication in the same request.\n  sources:\n  - https://developer.apple.com/library/archive/documentation/DataManagement/Conceptual/CloudKitWebServicesReference/SettingUpWebServices.html\n- name: managementToken\n  type: apiKey\n  in: header\n  parameter: null\n  scope: CloudKit Management API (schema operations via cktool / CKTool JS), not the database API\n  description: >-\n    Generated in the CloudKit Console under Settings for your user account and shown only once. cktool\n    stores management and user tokens in the macOS Keychain via `xcrun cktool save-token`.\n  sources:\n  - https://developer.apple.com/icloud/ck-tool/\nscopes:\n  published: false\n  note:\
  \ >-\n    No OAuth scopes exist. Authorization is decided by which database is addressed in the URL (public /\n    private / shared), by the container's per-record-type security roles configured in the CloudKit\n    Console, and by the record-level publicPermission value (NONE / READ_ONLY / READ_WRITE). Failures\n    surface as ACCESS_DENIED (HTTP 403).\nrotation:\n  documented: false\n  note: >-\n    No documented rotation or expiry policy for API tokens or server-to-server keys; both are revoked by\n    deleting them in the CloudKit Console. Only the user web-auth token has a stated lifetime.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/authentication/cloudkit-authentication.yml
summary_line: apiKey/signature · 4 schemes
tags:
- Apple
- Cloud Storage
- CloudKit
- Database
- iCloud
- Mobile
- Sync
- Web Services
---
