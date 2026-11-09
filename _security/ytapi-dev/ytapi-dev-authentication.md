---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ytapi Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: ytapi-dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ytapi-dev
provider_slug: ytapi-dev
scheme_count: 2
schemes:
- evidence: 'You can authenticate using either standard Bearer token or the X-API-Key header:'
  header: Authorization
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'You can authenticate using either standard Bearer token or the X-API-Key header:'
  header: X-API-Key
  location: header
  name: X-API-Key
  type: apiKey
slug: ytapi-dev-authentication
source_filename: ytapi-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ytapi.dev/authentication/
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ytapi.dev/authentication/\nsources:\n- https://docs.ytapi.dev/authentication/\n- https://docs.ytapi.dev/agent-setup/\n- https://docs.ytapi.dev/\n- https://docs.ytapi.dev/agent-setup/\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'You can authenticate using either standard Bearer token or the X-API-Key header:'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: X-API-Key\n  evidence: 'You can authenticate using either standard Bearer token or the X-API-Key header:'\n  location: header\n  header: X-API-Key\nnote: All authentication uses an API key that is obtained from the YTAPI Developer Dashboard.\ndocs: https://docs.ytapi.dev/authentication/\n"
source_yaml_url: https://artifacts.apis.io/ytapi-dev/authentication/ytapi-dev-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Video
- Transcripts
- YouTube
---
