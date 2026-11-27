---
anonymous_access: true
api_key_in: []
api_specs:
- filename: complyonsite-com-digital-waste-tracking-check-api-openapi.yml
  format: yaml
  label: ComplyOnSite Digital Waste Tracking Check API
  slug: complyonsite-com-digital-waste-tracking-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/complyonsite-com/openapi/complyonsite-com-digital-waste-tracking-check-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: ComplyOnSite Authentication
name_suffix: Authentication
oauth_flows: []
overview: ComplyOnSite declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ComplyOnSite
provider_slug: complyonsite-com
scheme_count: 1
schemes:
- applies_to:
  - https://mcp.complyonsite.com/mcp
  - https://complyonsite.com/api/digital-waste-tracking-check
  evidence: No account or key. It answers questions; it never saves, signs or sends anything.
  name: anonymous
  type: none
slug: complyonsite-com-authentication
source_filename: complyonsite-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://complyonsite.com/docs/mcp\n- https://complyonsite.com/docs\ndocs: https://complyonsite.com/docs/mcp\nschemes:\n- name: anonymous\n  type: none\n  applies_to:\n  - https://mcp.complyonsite.com/mcp\n  - https://complyonsite.com/api/digital-waste-tracking-check\n  evidence: \"No account or key. It answers questions; it never saves, signs or sends anything.\"\nsummary: Both machine-facing surfaces are anonymous. The MCP docs state \"No account, key, sign-in or cookie.\" and that the client should add the address \"with no authentication\". The OpenAPI for the Receipt of Waste checker declares no securitySchemes. The developer docs state \"Everything here is free and needs no account.\" Requests are counted against a per-IP limit (see rate-limits/).\n"
source_yaml_url: https://artifacts.apis.io/complyonsite-com/authentication/complyonsite-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Construction
- Health and Safety
- Environmental Compliance
- Waste Management
- RAMS
- MCP
- Open Data
---
