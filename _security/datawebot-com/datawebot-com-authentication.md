---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Datawebot Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: datawebot declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: datawebot
provider_slug: datawebot-com
scheme_count: 1
schemes:
- evidence: 'Store it as an application secret and send it as Authorization: Bearer <key>. Never put it in a URL.'
  header: Authorization
  how_to_obtain: Create a key in the dashboard; it starts with dwb_ and copy it.
  location: header
  name: Authorization
  type: http-bearer
slug: datawebot-com-authentication
source_filename: datawebot-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.datawebot.com/docs/api/quickstart
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.datawebot.com/docs/api/quickstart\nsources:\n- https://www.datawebot.com/docs/api/quickstart\n- https://www.datawebot.com/docs/api/reference\n- https://www.datawebot.com/SKILL.md\n- https://mcp.datawebot.com/setup.md\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Store it as an application secret and send it as Authorization: Bearer <key>. Never put it in a URL.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the dashboard; it starts with dwb_ and copy it.\ndocs: https://www.datawebot.com/docs/api/quickstart\n"
source_yaml_url: https://artifacts.apis.io/datawebot-com/authentication/datawebot-com-authentication.yml
summary_line: 1 scheme
tags:
- E-Commerce
- Artificial Intelligence
- Data
- Marketplace
---
