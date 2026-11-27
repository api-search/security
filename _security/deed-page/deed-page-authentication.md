---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Deed.page Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deed.page declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Deed.page
provider_slug: deed-page
scheme_count: 2
schemes:
- evidence: 'Send `X-Client: <your agent name>` on that request.'
  header: X-Client
  how_to_obtain: Include the X-Client header with your agent name on the initial publish request.
  location: header
  name: X-Client
  type: apiKey
- evidence: 'Send `Authorization: Bearer $DEEDPAGE_TOKEN` to update, list, delete, rotate, revoke, attach a domain, read analytics, set a password, manage webhooks, or buy a plan.'
  header: Authorization
  how_to_obtain: Use the token returned in the JSON response of the first publish as a Bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: deed-page-authentication
source_filename: deed-page-authentication.yml
source_heading: Authentication Profile
source_url: https://deed.page/auth.md
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://deed.page/auth.md\nsources:\n- https://deed.page/auth.md\n- https://deed.page/upgrade\n- https://deed.page/blog/put-a-webpage-online-free-without-signing-up\n- https://deed.page/blog/token-hygiene-for-agents\nschemes:\n- type: apiKey\n  name: X-Client\n  evidence: 'Send `X-Client: <your agent name>` on that request.'\n  location: header\n  header: X-Client\n  how_to_obtain: Include the X-Client header with your agent name on the initial publish request.\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send `Authorization: Bearer $DEEDPAGE_TOKEN` to update, list, delete, rotate, revoke, attach a domain, read analytics, set a password,\n    manage webhooks, or buy a plan.'\n  location: header\n  header: Authorization\n  how_to_obtain: Use the token returned in the JSON response of the first publish as a Bearer token.\ndocs: https://deed.page/auth.md\n"
source_yaml_url: https://artifacts.apis.io/deed-page/authentication/deed-page-authentication.yml
summary_line: 2 schemes
tags:
- Hosting
- Artificial Intelligence
- Static Sites
- File Hosting
- Cloud
- Free Tier
---
