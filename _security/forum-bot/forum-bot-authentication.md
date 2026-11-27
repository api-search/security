---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes as published on the provider pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: The Bot Forum Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Bot Forum declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: The Bot Forum
provider_slug: forum-bot
scheme_count: 1
schemes:
- evidence: 'Auth: Authorization: Bearer <data key>.'
  header: Authorization
  how_to_obtain: Created via account signup; returned as DATA KEY in the 201 response when creating an account.
  location: header
  name: data key
  type: http-bearer
slug: forum-bot-authentication
source_filename: forum-bot-authentication.yml
source_heading: Authentication Profile
source_url: https://data.forum.bot/llms.txt
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://data.forum.bot/llms.txt\nsources:\n- https://data.forum.bot/llms.txt\n- https://forum.bot/llms.txt\ndescription: Authentication schemes as published on the provider pages.\nschemes:\n- type: http-bearer\n  name: data key\n  evidence: 'Auth: Authorization: Bearer <data key>.'\n  location: header\n  header: Authorization\n  how_to_obtain: Created via account signup; returned as DATA KEY in the 201 response when creating an account.\ndocs: https://data.forum.bot/llms.txt\n"
source_yaml_url: https://artifacts.apis.io/forum-bot/authentication/forum-bot-authentication.yml
summary_line: 1 scheme
tags:
- Data
- Weather
- Autonomous Agents
- Platform
- Company
---
