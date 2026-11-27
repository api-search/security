---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: InkFE Authentication
name_suffix: Authentication
oauth_flows: []
overview: InkFE declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: InkFE
provider_slug: inkfe-com
scheme_count: 2
schemes:
- evidence: 'POST https://www.inkfe.com/api/mcp Authorization: Bearer <access token managed by your client>'
  header: Authorization
  how_to_obtain: Your app handles OAuth discovery and obtains an access token which is sent as a Bearer token in the Authorization header.
  location: header
  name: InkFE OAuth
  type: http-bearer
- evidence: Call start_guest_session and pass its private guestToken with design and checkout calls.
  header: Authorization
  how_to_obtain: Invoke the start_guest_session method (no arguments) to receive a guestToken, then include it as a Bearer token in the Authorization header.
  location: header
  name: Guest Token
  type: apiKey
slug: inkfe-com-authentication
source_filename: inkfe-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.inkfe.com/mcp/docs
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.inkfe.com/mcp/docs\nsources:\n- https://www.inkfe.com/mcp/docs\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: InkFE OAuth\n  evidence: 'POST https://www.inkfe.com/api/mcp Authorization: Bearer <access token managed by your client>'\n  location: header\n  header: Authorization\n  how_to_obtain: Your app handles OAuth discovery and obtains an access token which is sent as a Bearer token in the Authorization header.\n- type: apiKey\n  name: Guest Token\n  evidence: Call start_guest_session and pass its private guestToken with design and checkout calls.\n  location: header\n  header: Authorization\n  how_to_obtain: Invoke the start_guest_session method (no arguments) to receive a guestToken, then include it as a Bearer token in the Authorization\n    header.\nnote: OAuth flow URLs, specific scopes, and detailed flow types are not provided on the page;\
  \ those fields are left null or empty.\ndocs: https://www.inkfe.com/mcp/docs\n"
source_yaml_url: https://artifacts.apis.io/inkfe-com/authentication/inkfe-com-authentication.yml
summary_line: 2 schemes
tags:
- Printing
- E-Commerce
- Custom Design
- Marketing Materials
- United States
---
