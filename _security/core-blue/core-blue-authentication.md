---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: core.blue Authentication
name_suffix: Authentication
oauth_flows: []
overview: core.blue declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: core.blue
provider_slug: core-blue
scheme_count: 4
schemes:
- applies_to: https://mcp.core.blue/
  description: The manual and its skills are served by an MCP server over HTTP that needs no account and no key (https://core.blue/llms.txt).
  name: none (public adviser server)
  type: none
- applies_to: sandbox house doors returned by open_sandbox
  description: '"Connect your MCP client to the `modeller` door (streamable HTTP, no key: the address is the key)". "In a sandbox the lease or the sign-in is the key." Lease format: `sb_` and 26 characters.'
  docs: https://core.blue/topics/the-sandbox.md
  name: sandbox lease
  type: capability-url
- applies_to: https://try.core.blue/ (live, account-less sign-in) and a house of your own (planned)
  description: '"The client finds out by itself where to sign in (the way MCP prescribes, with OAuth), opens a browser window, and the person you act for clicks "Erlauben" there." try.core.blue advertises OAuth protected-resource metadata and answers unauthenticated calls with 401 and a Bearer resource_metadata challenge.'
  name: MCP OAuth sign-in
  status: live on try.core.blue; planned for houses of your own
  type: oauth2
- applies_to: a house of your own, for scripts and services
  description: '"A resident makes it a key (`create_key` at the keys door, planned with the gate); it sends `Authorization: Bearer cb_…` with every request."'
  name: house key (bearer)
  scheme: bearer
  status: planned
  type: http
slug: core-blue-authentication
source_filename: core-blue-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://core.blue/topics/connecting-to-your-house.md\ndocs: https://core.blue/topics/connecting-to-your-house.md\nschemes:\n- name: none (public adviser server)\n  type: none\n  applies_to: https://mcp.core.blue/\n  description: The manual and its skills are served by an MCP server over HTTP that needs no account and no key (https://core.blue/llms.txt).\n- name: sandbox lease\n  type: capability-url\n  applies_to: sandbox house doors returned by open_sandbox\n  description: >-\n    \"Connect your MCP client to the `modeller` door (streamable HTTP, no key: the address is the key)\".\n    \"In a sandbox the lease or the sign-in is the key.\" Lease format: `sb_` and 26 characters.\n  docs: https://core.blue/topics/the-sandbox.md\n- name: MCP OAuth sign-in\n  type: oauth2\n  applies_to: https://try.core.blue/ (live, account-less sign-in) and a house of your own (planned)\n  description: >-\n    \"The client finds out by itself\
  \ where to sign in (the way MCP prescribes, with OAuth), opens a browser\n    window, and the person you act for clicks \"Erlauben\" there.\" try.core.blue advertises OAuth\n    protected-resource metadata and answers unauthenticated calls with 401 and a Bearer resource_metadata challenge.\n  status: live on try.core.blue; planned for houses of your own\n- name: house key (bearer)\n  type: http\n  scheme: bearer\n  applies_to: a house of your own, for scripts and services\n  description: >-\n    \"A resident makes it a key (`create_key` at the keys door, planned with the gate); it sends\n    `Authorization: Bearer cb_…` with every request.\"\n  status: planned\n"
source_yaml_url: https://artifacts.apis.io/core-blue/authentication/core-blue-authentication.yml
summary_line: 4 schemes
tags:
- Company
- AI Agents
- Agent Memory
- MCP
- Database
- Knowledge Management
- Provenance
---
