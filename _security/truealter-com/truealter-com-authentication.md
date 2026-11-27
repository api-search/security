---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for ~Alter as documented
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ~Alter Authentication
name_suffix: Authentication
oauth_flows: []
overview: ~Alter declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ~Alter
provider_slug: truealter-com
scheme_count: 2
schemes:
- evidence: 'Authorization: Bearer <access_token>'
  header: Authorization
  how_to_obtain: Obtain via the /auth/login endpoint (or /auth/register which auto‑logs in). The access token is returned in the response body and the refresh token is set as an HttpOnly cookie.
  location: header
  name: JWT Bearer Token
  type: http-bearer
- evidence: 'Authorization: Bearer <capability_token>'
  header: Authorization
  how_to_obtain: Connect via OAuth (browser connector or programmatic OAuth flow) to receive a capability token scoped per tool. The token is then sent in the Authorization header.
  location: header
  name: OAuth‑bearer capability
  type: http-bearer
slug: truealter-com-authentication
source_filename: truealter-com-authentication.yml
source_heading: Authentication Profile
source_url: https://truealter.com/docs/authentication
source_yaml: "generated: '2026-11-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://truealter.com/docs/authentication\nsources:\n- https://truealter.com/docs/authentication\n- https://truealter.com/docs/mcp\n- https://truealter.com/docs/authentication.md\n- https://truealter.com/docs/rest-api/auth\ndescription: Authentication methods for ~Alter as documented\nschemes:\n- type: http-bearer\n  name: JWT Bearer Token\n  evidence: 'Authorization: Bearer <access_token>'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain via the /auth/login endpoint (or /auth/register which auto‑logs in). The access token is returned in the response body\n    and the refresh token is set as an HttpOnly cookie.\n- type: http-bearer\n  name: OAuth‑bearer capability\n  evidence: 'Authorization: Bearer <capability_token>'\n  location: header\n  header: Authorization\n  how_to_obtain: Connect via OAuth (browser connector or programmatic OAuth flow) to receive a\
  \ capability token scoped per tool. The token is\n    then sent in the Authorization header.\nnote: OAuth flow URLs and scopes are not listed on the pages, so they are omitted.\ndocs: https://truealter.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/truealter-com/authentication/truealter-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
