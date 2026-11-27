---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Emora Health as documented on https://www.emorahealth.com/auth.md
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Emora Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Emora Health declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Emora Health
provider_slug: emorahealth-com
scheme_count: 1
schemes:
- authorize_url: https://www.emorahealth.com/api/oauth/auth
  evidence: OAuth 2.1, for the ops surface. `POST https://www.emorahealth.com/mcp/ops` requires a Bearer token scoped `mcp`.
  flows:
  - authorization_code
  - client_credentials
  header: Authorization
  how_to_obtain: Dynamic client registration at `POST https://www.emorahealth.com/api/oauth/reg` (no initial access token) then use the authorization code flow with PKCE or client_credentials grant to obtain a token.
  location: header
  name: OAuth 2.1 Bearer
  scopes:
  - mcp
  - offline_access
  type: http-bearer
slug: emorahealth-com-authentication
source_filename: emorahealth-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.emorahealth.com/auth.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.emorahealth.com/auth.md\nsources:\n- https://www.emorahealth.com/auth.md\ndescription: Authentication methods for Emora Health as documented on https://www.emorahealth.com/auth.md\nschemes:\n- type: http-bearer\n  name: OAuth 2.1 Bearer\n  evidence: OAuth 2.1, for the ops surface. `POST https://www.emorahealth.com/mcp/ops` requires a Bearer token scoped `mcp`.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  - client_credentials\n  authorize_url: https://www.emorahealth.com/api/oauth/auth\n  scopes:\n  - mcp\n  - offline_access\n  how_to_obtain: Dynamic client registration at `POST https://www.emorahealth.com/api/oauth/reg` (no initial access token) then use the authorization\n    code flow with PKCE or client_credentials grant to obtain a token.\ndocs: https://www.emorahealth.com/auth.md\nnote: 1 extracted row(s) were dropped because\
  \ their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/emorahealth-com/authentication/emorahealth-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Mental Health
- Telehealth
- Pediatrics
- Therapy
---
