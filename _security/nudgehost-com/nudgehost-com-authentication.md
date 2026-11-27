---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods as published on the page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: NudgeHost Authentication
name_suffix: Authentication
oauth_flows: []
overview: NudgeHost declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: NudgeHost
provider_slug: nudgehost-com
scheme_count: 1
schemes:
- evidence: '"bearer_methods_supported": ["header"]'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: nudgehost-com-authentication
source_filename: nudgehost-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.nudgehost.com/.well-known/oauth-protected-resource
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.nudgehost.com/.well-known/oauth-protected-resource\nsources:\n- https://www.nudgehost.com/.well-known/oauth-protected-resource\ndescription: Authentication methods as published on the page.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '\"bearer_methods_supported\": [\"header\"]'\n  location: header\n  header: Authorization\ndocs: https://www.nudgehost.com/.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/nudgehost-com/authentication/nudgehost-com-authentication.yml
summary_line: 1 scheme
tags:
- File Hosting
- Cloud
- Artificial Intelligence
- Sharing
---
