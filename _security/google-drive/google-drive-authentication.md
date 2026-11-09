---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-drive-files-api-openapi.yml
  format: yaml
  label: Google Drive Files API
  slug: google-drive-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-files-api-openapi.yml
- filename: google-drive-about-api-openapi.yml
  format: yaml
  label: Google Drive About API
  slug: google-drive-about-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-about-api-openapi.yml
- filename: google-drive-accessproposals-api-openapi.yml
  format: yaml
  label: Google Drive Accessproposals API
  slug: google-drive-accessproposals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-accessproposals-api-openapi.yml
- filename: google-drive-approvals-api-openapi.yml
  format: yaml
  label: Google Drive Approvals API
  slug: google-drive-approvals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-approvals-api-openapi.yml
- filename: google-drive-apps-api-openapi.yml
  format: yaml
  label: Google Drive Apps API
  slug: google-drive-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-apps-api-openapi.yml
- filename: google-drive-changes-api-openapi.yml
  format: yaml
  label: Google Drive Changes API
  slug: google-drive-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-changes-api-openapi.yml
- filename: google-drive-channels-api-openapi.yml
  format: yaml
  label: Google Drive Channels API
  slug: google-drive-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-channels-api-openapi.yml
- filename: google-drive-comments-api-openapi.yml
  format: yaml
  label: Google Drive Comments API
  slug: google-drive-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-comments-api-openapi.yml
- filename: google-drive-drives-api-openapi.yml
  format: yaml
  label: Google Drive Drives API
  slug: google-drive-drives-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-drives-api-openapi.yml
- filename: google-drive-operations-api-openapi.yml
  format: yaml
  label: Google Drive Operations API
  slug: google-drive-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-operations-api-openapi.yml
- filename: google-drive-permissions-api-openapi.yml
  format: yaml
  label: Google Drive Permissions API
  slug: google-drive-permissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-permissions-api-openapi.yml
- filename: google-drive-replies-api-openapi.yml
  format: yaml
  label: Google Drive Replies API
  slug: google-drive-replies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-replies-api-openapi.yml
- filename: google-drive-revisions-api-openapi.yml
  format: yaml
  label: Google Drive Revisions API
  slug: google-drive-revisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-revisions-api-openapi.yml
- filename: google-drive-teamdrives-api-openapi.yml
  format: yaml
  label: Google Drive Teamdrives API
  slug: google-drive-teamdrives-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-drive/openapi/google-drive-teamdrives-api-openapi.yml
auth_types:
- oauth2
- apiKey
description: Authentication profile for the Google Drive API v3. The captured OpenAPI does not declare securitySchemes, so this profile was upgraded from Google's Drive auth documentation. All Drive API requests require an OAuth 2.0 access token (three-legged for user data; two-legged service-account / domain-wide delegation for Workspace). API keys authenticate only fully public file reads. Scope detail lives in scopes/google-drive-scopes.yml.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Google Drive Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
- jwt-bearer
overview: Google Drive secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, deviceCode, and jwt-bearer flow(s).
provider_name: Google Drive
provider_slug: google-drive
scheme_count: 2
schemes:
- discovery: well-known/google-drive-openid-configuration.json
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    refresh: true
    tokenUrl: https://oauth2.googleapis.com/token
  - deviceAuthorizationUrl: https://oauth2.googleapis.com/device/code
    flow: deviceCode
    tokenUrl: https://oauth2.googleapis.com/token
  - description: JWT-bearer (RFC 7523) service-account flow, optionally with Workspace domain-wide delegation to impersonate users.
    flow: serviceAccount
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  revocation: https://oauth2.googleapis.com/revoke
  sources:
  - docs
  type: oauth2
- in: query
  name: ApiKey
  note: Authenticates access to publicly shared files only; cannot access private user data.
  parameter: key
  sources:
  - docs
  type: apiKey
slug: google-drive-authentication
source_filename: google-drive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/google-drive-openapi.yml\ndocs: https://developers.google.com/workspace/drive/api/guides/about-auth\ndescription: >-\n  Authentication profile for the Google Drive API v3. The captured OpenAPI does\n  not declare securitySchemes, so this profile was upgraded from Google's Drive\n  auth documentation. All Drive API requests require an OAuth 2.0 access token\n  (three-legged for user data; two-legged service-account / domain-wide delegation\n  for Workspace). API keys authenticate only fully public file reads. Scope detail\n  lives in scopes/google-drive-scopes.yml.\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [query]\n  oauth2_flows: [authorizationCode, deviceCode, jwt-bearer]\nschemes:\n  - name: OAuth2\n    type: oauth2\n    sources: [docs]\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\n\
  \        refresh: true\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://oauth2.googleapis.com/device/code\n        tokenUrl: https://oauth2.googleapis.com/token\n      - flow: serviceAccount\n        description: >-\n          JWT-bearer (RFC 7523) service-account flow, optionally with Workspace\n          domain-wide delegation to impersonate users.\n        tokenUrl: https://oauth2.googleapis.com/token\n    revocation: https://oauth2.googleapis.com/revoke\n    discovery: well-known/google-drive-openid-configuration.json\n  - name: ApiKey\n    type: apiKey\n    in: query\n    parameter: key\n    sources: [docs]\n    note: Authenticates access to publicly shared files only; cannot access private user data.\n"
source_yaml_url: https://artifacts.apis.io/google-drive/authentication/google-drive-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Cloud Storage
- Collaboration
- Document Management
- Drives
- File
- Google
- Storage
---
