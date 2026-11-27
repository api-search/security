---
anonymous_access: true
api_key_in: []
api_specs:
- filename: coronet-one-confirm-checkout-api-openapi.yml
  format: yaml
  label: Coronet Arcade Confirm Checkout API
  slug: coronet-one-confirm-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coronet-one/openapi/coronet-one-confirm-checkout-api-openapi.yml
- filename: coronet-one-create-checkout-api-openapi.yml
  format: yaml
  label: Coronet Arcade Create Checkout API
  slug: coronet-one-create-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coronet-one/openapi/coronet-one-create-checkout-api-openapi.yml
- filename: coronet-one-mcp-api-openapi.yml
  format: yaml
  label: Coronet Arcade MCP API
  slug: coronet-one-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coronet-one/openapi/coronet-one-mcp-api-openapi.yml
- filename: coronet-one-restore-purchase-api-openapi.yml
  format: yaml
  label: Coronet Arcade Restore Purchase API
  slug: coronet-one-restore-purchase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coronet-one/openapi/coronet-one-restore-purchase-api-openapi.yml
- filename: coronet-one-site-api-openapi.yml
  format: yaml
  label: Coronet Arcade Site API
  slug: coronet-one-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coronet-one/openapi/coronet-one-site-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Coronet Arcade Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coronet Arcade declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Coronet Arcade
provider_slug: coronet-one
scheme_count: 1
schemes:
- applies_to:
  - getSiteFacts
  - mcpInfo
  - mcpRpc
  description: Anonymous read of /api/site, /api/mcp, /llms.txt -- Supported — no credential
  evidence: https://coronet.one/auth.md
  name: anonymous
  type: none
slug: coronet-one-authentication
source_filename: coronet-one-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coronet.one/auth.md\ndocs: https://coronet.one/auth.md\nsummary: >-\n  The OpenAPI (https://coronet.one/openapi.json) declares no securitySchemes. The provider's auth.md states the\n  public surface is anonymous: \"There is no OAuth stack and no agent user-registration API.\" Player sign-in\n  (Google, Apple, emailed magic link) is a separate optional human flow, not an API credential.\nschemes:\n- name: anonymous\n  type: none\n  description: \"Anonymous read of /api/site, /api/mcp, /llms.txt -- Supported — no credential\"\n  applies_to: [getSiteFacts, mcpInfo, mcpRpc]\n  evidence: https://coronet.one/auth.md\noauth: not offered (auth.md - \"OAuth / OIDC login | Not offered\")\nagent_registration: not offered (auth.md - \"Registration required | No\")\n"
source_yaml_url: https://artifacts.apis.io/coronet-one/authentication/coronet-one-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Games
- Puzzles
- Word Games
- Logic Puzzles
- MCP
- AI Agents
---
