---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Razi Pro Authentication
name_suffix: Authentication
oauth_flows: []
overview: razi-pro declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: razi-pro
provider_slug: razi-pro
scheme_count: 1
schemes:
- authorize_url: https://stg-id.uaepass.ae/idshub/authorize
  evidence: UAE Pass is an OAuth 2.0 provider, and that sentence will cost you a day if you believe all of it.
  how_to_obtain: Use Basic authentication with base64‑encoded "client_id:client_secret" in the Authorization header and send the token request parameters in the query string as documented.
  name: UAE Pass
  scopes:
  - urn:uae:digitalid:profile:general
  - urn:uae:digitalid:profile:general:profileType
  - urn:uae:digitalid:profile:general:unifiedId
  type: oauth2
slug: razi-pro-authentication
source_filename: razi-pro-authentication.yml
source_heading: Authentication Profile
source_url: https://www.razi.pro/blog/uae-pass-integration-dotnet.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.razi.pro/blog/uae-pass-integration-dotnet.md\nsources:\n- https://www.razi.pro/blog/uae-pass-integration-dotnet.md\n- https://www.razi.pro/help/account-and-sign-in.md\n- https://www.razi.pro/tools/jwt-decoder/docs\n- https://www.razi.pro/tools/jwt-decoder\nschemes:\n- type: oauth2\n  name: UAE Pass\n  evidence: UAE Pass is an OAuth 2.0 provider, and that sentence will cost you a day if you believe all of it.\n  authorize_url: https://stg-id.uaepass.ae/idshub/authorize\n  scopes:\n  - urn:uae:digitalid:profile:general\n  - urn:uae:digitalid:profile:general:profileType\n  - urn:uae:digitalid:profile:general:unifiedId\n  how_to_obtain: Use Basic authentication with base64‑encoded \"client_id:client_secret\" in the Authorization header and send the token request\n    parameters in the query string as documented.\ndocs: https://www.razi.pro/blog/uae-pass-integration-dotnet.md\n"
source_yaml_url: https://artifacts.apis.io/razi-pro/authentication/razi-pro-authentication.yml
summary_line: 1 scheme
tags:
- Developer Tools
- Tech Blog
- Free Resources
- Community
- AI Tools
---
