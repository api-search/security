---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for LeadMarina APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LeadMarina Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeadMarina declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LeadMarina
provider_slug: leadmarina
scheme_count: 2
schemes:
- evidence: API keys as bearer tokens — how every LeadMarina API request authenticates.
  header: Authorization
  location: header
  name: Bearer token
  type: http-bearer
- evidence: Send it as a bearer token (or the x-api-key header).
  header: x-api-key
  location: header
  name: API key header
  type: apiKey
slug: leadmarina-authentication
source_filename: leadmarina-authentication.yml
source_heading: Authentication Profile
source_url: https://leadmarina.com/docs/authentication
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://leadmarina.com/docs/authentication\nsources:\n- https://leadmarina.com/docs/authentication\n- https://leadmarina.com/docs/mcp\n- https://leadmarina.com/docs/quick-start\ndescription: Authentication methods for LeadMarina APIs\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: API keys as bearer tokens — how every LeadMarina API request authenticates.\n  location: header\n  header: Authorization\n- type: apiKey\n  name: API key header\n  evidence: Send it as a bearer token (or the x-api-key header).\n  location: header\n  header: x-api-key\ndocs: https://leadmarina.com/docs/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/leadmarina/authentication/leadmarina-authentication.yml
summary_line: 2 schemes
tags:
- Email Verification
- Phone Verification
- Outbound Outreach
---
