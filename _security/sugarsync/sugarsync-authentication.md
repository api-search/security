---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sugarsync-openapi-generated.yml
  format: yaml
  label: SugarSync API
  slug: sugarsync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sugarsync/openapi/_ae-authored/sugarsync-openapi-generated.yml
auth_types: []
description: SugarSync uses a custom token‑based authentication flow. A client first obtains a refresh token by POSTing XML credentials (username, password, application ID, accessKeyId, privateAccessKey) to the app‑authorization endpoint. The refresh token is returned in the Location response header. The client then exchanges the refresh token for an access token by POSTing XML (accessKeyId, privateAccessKey, refreshToken) to the authorization endpoint. The access token is also returned in the Location response header and must be sent in the Authorization header of subsequent API calls.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Sugarsync Authentication
name_suffix: Authentication
oauth_flows: []
overview: SugarSync declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: SugarSync
provider_slug: sugarsync
scheme_count: 2
schemes:
- evidence: To create a refresh token, an application submits an HTTP POST request to the app-authorization endpoint.
  how_to_obtain: POST XML containing username, password, application ID, accessKeyId, privateAccessKey to https://api.sugarsync.com/app-authorization; token returned in Location header.
  location: body
  name: Refresh Token
  type: other
- evidence: To create an access token, an application submits an HTTP POST request to the authorization endpoint.
  how_to_obtain: POST XML containing accessKeyId, privateAccessKey, refreshToken to https://api.sugarsync.com/authorization; token returned in Location header and used in Authorization header of API calls.
  location: body
  name: Access Token
  type: other
slug: sugarsync-authentication
source_filename: sugarsync-authentication.yml
source_heading: Authentication Profile
source_url: https://www1.sugarsync.com/developer/api/auth-resource/
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www1.sugarsync.com/developer/api/auth-resource/\nsources:\n- https://www1.sugarsync.com/developer/api/auth-resource/\n- https://www1.sugarsync.com/developer/api/method/create-refresh-token/\n- https://www1.sugarsync.com/developer/api/method/create-auth-token/\n- https://www1.sugarsync.com/developer/get-auth-token-example/\ndescription: SugarSync uses a custom token‑based authentication flow. A client first obtains a refresh token by POSTing XML credentials (username,\n  password, application ID, accessKeyId, privateAccessKey) to the app‑authorization endpoint. The refresh token is returned in the Location response\n  header. The client then exchanges the refresh token for an access token by POSTing XML (accessKeyId, privateAccessKey, refreshToken) to the\n  authorization endpoint. The access token is also returned in the Location response header and must be sent in the Authorization\
  \ header of subsequent\n  API calls.\nschemes:\n- type: other\n  name: Refresh Token\n  evidence: To create a refresh token, an application submits an HTTP POST request to the app-authorization endpoint.\n  location: body\n  how_to_obtain: POST XML containing username, password, application ID, accessKeyId, privateAccessKey to https://api.sugarsync.com/app-authorization;\n    token returned in Location header.\n- type: other\n  name: Access Token\n  evidence: To create an access token, an application submits an HTTP POST request to the authorization endpoint.\n  location: body\n  how_to_obtain: POST XML containing accessKeyId, privateAccessKey, refreshToken to https://api.sugarsync.com/authorization; token returned in\n    Location header and used in Authorization header of API calls.\ndocs: https://www1.sugarsync.com/developer/api/auth-resource/\n"
source_yaml_url: https://artifacts.apis.io/sugarsync/authentication/sugarsync-authentication.yml
summary_line: 2 schemes
tags:
- Cloud Storage
- File Sync
- Backup
- Collaboration
- Business
---
