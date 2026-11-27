---
anonymous_access: false
api_key_in: []
auth_types: []
description: Engram uses a Bearer token passed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Engram Authentication
name_suffix: Authentication
oauth_flows: []
overview: Engram declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Engram
provider_slug: engram-page
scheme_count: 1
schemes:
- evidence: Section titled “Authorizations” bearerAuth
  header: Authorization
  location: header
  name: bearerAuth
  type: http-bearer
slug: engram-page-authentication
source_filename: engram-page-authentication.yml
source_heading: Authentication Profile
source_url: https://engram.page/docs/api/operations/tags/api-keys
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://engram.page/docs/api/operations/tags/api-keys\nsources:\n- https://engram.page/docs/api/operations/tags/api-keys\n- https://engram.page/docs/api/operations/apikeys-revoke\n- https://engram.page/docs/api/operations/apikeys-list\n- https://engram.page/docs/api/operations/apikeys-create\ndescription: Engram uses a Bearer token passed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: bearerAuth\n  evidence: Section titled “Authorizations” bearerAuth\n  location: header\n  header: Authorization\ndocs: https://engram.page/docs/api/operations/tags/api-keys\n"
source_yaml_url: https://artifacts.apis.io/engram-page/authentication/engram-page-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Personal Data
- Note Taking
- Knowledge Base
- Privacy
---
