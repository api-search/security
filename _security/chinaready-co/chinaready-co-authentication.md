---
anonymous_access: true
api_key_in: []
api_specs:
- filename: chinaready-co-assistant-api-openapi.yml
  format: yaml
  label: Chinaready Assistant API
  slug: chinaready-co-assistant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chinaready-co/openapi/chinaready-co-assistant-api-openapi.yml
- filename: chinaready-co-contact-api-openapi.yml
  format: yaml
  label: Chinaready Contact API
  slug: chinaready-co-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chinaready-co/openapi/chinaready-co-contact-api-openapi.yml
- filename: chinaready-co-intake-api-openapi.yml
  format: yaml
  label: Chinaready Intake API
  slug: chinaready-co-intake-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chinaready-co/openapi/chinaready-co-intake-api-openapi.yml
- filename: chinaready-co-search-api-openapi.yml
  format: yaml
  label: Chinaready Search API
  slug: chinaready-co-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chinaready-co/openapi/chinaready-co-search-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Chinaready Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chinaready declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Chinaready
provider_slug: chinaready-co
scheme_count: 1
schemes:
- applies_to:
  - postContact
  - postIntake
  - postAssistantChat
  - aiSearch
  - postSiteSearch
  - https://mcp.chinaready.co/mcp
  description: All public REST endpoints and the MCP server are unauthenticated. The docs say "No API keys, no sign-in." and, for the MCP server, "No sign-in — no keys, no OAuth".
  type: none
slug: chinaready-co-authentication
source_filename: chinaready-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://chinaready.co/docs/api/\ndocs: https://chinaready.co/docs/api/\nschemes:\n- type: none\n  description: All public REST endpoints and the MCP server are unauthenticated. The docs say \"No API keys, no sign-in.\" and, for the MCP server, \"No sign-in — no keys, no OAuth\".\n  applies_to: [postContact, postIntake, postAssistantChat, aiSearch, postSiteSearch, https://mcp.chinaready.co/mcp]\nsummary: The OpenAPI (openapi/chinaready-co-openapi.yml, info.version 0.5.0) declares no securitySchemes, and its info.description says \"no public OAuth yet\".\n"
source_yaml_url: https://artifacts.apis.io/chinaready-co/authentication/chinaready-co-authentication.yml
summary_line: 1 scheme
tags:
- Company
- China
- Market Entry
- Content Delivery
- Hosting
- Compliance
- Mobile App Distribution
- Network Diagnostics
- MCP
---
