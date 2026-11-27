---
anonymous_access: false
api_key_in: []
api_specs:
- filename: commonspecs-com-openapi-generated.yml
  format: yaml
  label: commonspecs API
  slug: commonspecs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commonspecs-com/openapi/_ae-authored/commonspecs-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: commonspecs Authentication
name_suffix: Authentication
oauth_flows: []
overview: commonspecs declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: commonspecs
provider_slug: commonspecs-com
scheme_count: 2
schemes:
- evidence: 'Send the bearer token in a header: Authorization: Bearer cs_live_…'
  header: 'Authorization: Bearer cs_live_…'
  name: bearer
  obtain: API token generated on the user's profile at https://commonspecs.com/account/
  scheme: bearer
  token_prefix: cs_live_
  transport: REST (https://api.commonspecs.com/v1/*)
  type: http
- evidence: The connection carries its own OAuth sign-in; no token needed.
  name: mcp-oauth
  note: OAuth flow details (endpoints, scopes) are not published in the docs; not probed per probe-safety rules.
  source: https://github.com/commonspecs/skills/blob/HEAD/skills/commonspecs/SKILL.md
  transport: MCP (https://api.commonspecs.com/mcp)
  type: oauth2
slug: commonspecs-com-authentication
source_filename: commonspecs-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: commonspecs authentication\ngenerated: '2026-11-04'\nmethod: searched\nsource: https://commonspecs.com/docs/api/\ndocs: https://commonspecs.com/docs/api/\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  transport: REST (https://api.commonspecs.com/v1/*)\n  token_prefix: cs_live_\n  header: 'Authorization: Bearer cs_live_…'\n  obtain: API token generated on the user's profile at https://commonspecs.com/account/\n  evidence: 'Send the bearer token in a header: Authorization: Bearer cs_live_…'\n- name: mcp-oauth\n  type: oauth2\n  transport: MCP (https://api.commonspecs.com/mcp)\n  evidence: The connection carries its own OAuth sign-in; no token needed.\n  source: https://github.com/commonspecs/skills/blob/HEAD/skills/commonspecs/SKILL.md\n  note: OAuth flow details (endpoints, scopes) are not published in the docs; not probed per probe-safety rules.\ntest_keys: none published; only the cs_live_ prefix is documented.\n"
source_yaml_url: https://artifacts.apis.io/commonspecs-com/authentication/commonspecs-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Product Data
- Product Specifications
- Price Comparison
- AI Agents
- MCP
- Agent Skills
- E-Commerce
---
