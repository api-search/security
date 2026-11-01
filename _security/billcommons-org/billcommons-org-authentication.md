---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Bill Commons API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Billcommons Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: billcommons-org declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: billcommons-org
provider_slug: billcommons-org
scheme_count: 2
schemes:
- evidence: Send the key as a Bearer token. X-Api-Key is also accepted for clients that can't set Authorization.
  header: Authorization
  how_to_obtain: Request a sign-in link by email. No password or account form. First sign-in mints your Developer key automatically.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: Send the key as a Bearer token. X-Api-Key is also accepted for clients that can't set Authorization.
  header: X-Api-Key
  how_to_obtain: Request a sign-in link by email. No password or account form. First sign-in mints your Developer key automatically.
  location: header
  name: X-Api-Key header
  type: apiKey
slug: billcommons-org-authentication
source_filename: billcommons-org-authentication.yml
source_heading: Authentication Profile
source_url: https://billcommons.org/docs/api-keys
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://billcommons.org/docs/api-keys\nsources:\n- https://billcommons.org/docs/api-keys\n- https://billcommons.org/docs/chatgpt\n- https://billcommons.org/docs/mcp\ndescription: Authentication methods for Bill Commons API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Send the key as a Bearer token. X-Api-Key is also accepted for clients that can't set Authorization.\n  location: header\n  header: Authorization\n  how_to_obtain: Request a sign-in link by email. No password or account form. First sign-in mints your Developer key automatically.\n- type: apiKey\n  name: X-Api-Key header\n  evidence: Send the key as a Bearer token. X-Api-Key is also accepted for clients that can't set Authorization.\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Request a sign-in link by email. No password or account form. First sign-in mints your Developer key automatically.\n\
  note: Public MCP endpoint requires no authentication.\ndocs: https://billcommons.org/docs/api-keys\n"
source_yaml_url: https://artifacts.apis.io/billcommons-org/authentication/billcommons-org-authentication.yml
summary_line: 2 schemes
tags:
- Legislative data
- State bills
- API
- Open source
- Research tools
---
