---
api_key_in:
- query
api_specs:
- filename: google-drive-openapi.yml
  format: yaml
  label: Google Drive API v3
  slug: google-drive-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-drive/refs/heads/main/openapi/google-drive-openapi.yml
auth_types:
- oauth2
- apiKey
description: Authentication profile for the Google Drive API v3. The captured OpenAPI does not declare securitySchemes, so this profile was upgraded from Google's Drive auth documentation. All Drive API requests require an OAuth 2.0 access token (three-legged for user data; two-legged service-account / domain-wide delegation for Workspace). API keys authenticate only fully public file reads. Scope detail lives in scopes/google-drive-scopes.yml.
kind: authentication
layout: security
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
  name: key
  note: Authenticates access to publicly shared files only; cannot access private user data.
  sources:
  - docs
  type: apiKey
slug: google-drive-authentication
source_filename: google-drive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/google-drive-openapi.yml\ndocs: https://developers.google.com/workspace/drive/api/guides/about-auth\ndescription: >-\n  Authentication profile for the Google Drive API v3. The captured OpenAPI does\n  not declare securitySchemes, so this profile was upgraded from Google's Drive\n  auth documentation. All Drive API requests require an OAuth 2.0 access token\n  (three-legged for user data; two-legged service-account / domain-wide delegation\n  for Workspace). API keys authenticate only fully public file reads. Scope detail\n  lives in scopes/google-drive-scopes.yml.\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [query]\n  oauth2_flows: [authorizationCode, deviceCode, jwt-bearer]\nschemes:\n  - name: OAuth2\n    type: oauth2\n    sources: [docs]\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\n\
  \        refresh: true\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://oauth2.googleapis.com/device/code\n        tokenUrl: https://oauth2.googleapis.com/token\n      - flow: serviceAccount\n        description: >-\n          JWT-bearer (RFC 7523) service-account flow, optionally with Workspace\n          domain-wide delegation to impersonate users.\n        tokenUrl: https://oauth2.googleapis.com/token\n    revocation: https://oauth2.googleapis.com/revoke\n    discovery: well-known/google-drive-openid-configuration.json\n  - name: ApiKey\n    type: apiKey\n    in: query\n    name: key\n    sources: [docs]\n    note: Authenticates access to publicly shared files only; cannot access private user data.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-drive/refs/heads/main/authentication/google-drive-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Cloud Storage
- Collaboration
- Document Management
- Drive
- Files
- Google
- Storage
---
