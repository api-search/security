---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for Mainline coding agents
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mainline Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mainline declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mainline
provider_slug: mainline-dev
scheme_count: 1
schemes:
- evidence: Make a personal token under Profile, then Coding agents, ticking the teams it may read.
  header: Authorization
  how_to_obtain: Make a personal token under Profile, then Coding agents, ticking the teams it may read.
  location: header
  name: Personal Token
  type: http-bearer
slug: mainline-dev-authentication
source_filename: mainline-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://mainline.dev/docs/coding-agents
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mainline.dev/docs/coding-agents\nsources:\n- https://mainline.dev/docs/coding-agents\ndescription: Authentication for Mainline coding agents\nschemes:\n- type: http-bearer\n  name: Personal Token\n  evidence: Make a personal token under Profile, then Coding agents, ticking the teams it may read.\n  location: header\n  header: Authorization\n  how_to_obtain: Make a personal token under Profile, then Coding agents, ticking the teams it may read.\ndocs: https://mainline.dev/docs/coding-agents\n"
source_yaml_url: https://artifacts.apis.io/mainline-dev/authentication/mainline-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Project Management
- Continuous Delivery
- DevOps
- Software-as-a-Service
---
