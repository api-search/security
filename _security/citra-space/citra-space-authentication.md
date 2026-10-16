---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for the Citra Space API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Citra Space Authentication
name_suffix: Authentication
oauth_flows: []
overview: Citra Space declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Citra Space
provider_slug: citra-space
scheme_count: 1
schemes:
- evidence: All API requests require authentication using your personal access token in the Authorization header as a Bearer token.
  header: Authorization
  how_to_obtain: Create a personal access token in the Citra Space app under User Settings → Access Tokens.
  location: header
  name: Bearer token
  type: http-bearer
slug: citra-space-authentication
source_filename: citra-space-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.citra.space/citra-space-app-api/user/access-tokens.html
source_yaml: "generated: '2026-10-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.citra.space/citra-space-app-api/user/access-tokens.html\nsources:\n- https://docs.citra.space/citra-space-app-api/user/access-tokens.html\n- https://docs.citra.space/guides-and-tutorials/api-quickstart-guide.html\n- https://docs.citra.space/citrasense/GettingStarted.html\n- https://docs.citra.space/guides-and-tutorials/api-quickstart-guide\ndescription: Authentication for the Citra Space API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: All API requests require authentication using your personal access token in the Authorization header as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a personal access token in the Citra Space app under User Settings → Access Tokens.\nnote: No OAuth2 flows, apiKey, or other authentication schemes are documented on the provided pages.\ndocs: https://docs.citra.space/citra-space-app-api/user/access-tokens.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citra-space/refs/heads/main/authentication/citra-space-authentication.yml
summary_line: 1 scheme
tags:
- Space Domain Awareness
- Hardware
- Software
- Infrastructure
- Platforms
- Applications
- Technology
---
