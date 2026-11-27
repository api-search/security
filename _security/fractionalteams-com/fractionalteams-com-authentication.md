---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fractionalteams-com-api-openapi.json
  format: json
  label: Fractional Teams Portal API API
  slug: fractional-teams-portal-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fractionalteams-com/openapi/_original/fractionalteams-com-api-openapi.json
auth_types: []
description: Authentication schemes for Fractional Teams Portal API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Fractional Teams Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fractional Teams declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Fractional Teams
provider_slug: fractionalteams-com
scheme_count: 2
schemes:
- evidence: 'The portal uses **per-user bearer API keys**, not OAuth: there is no authorization server, no `agent_auth` endpoint and no dynamic `register_uri`: a human issues the key.'
  header: Authorization
  how_to_obtain: Human creates the key on the portal account page (https://portal.fractionalteams.com/account) → API keys → Create key and copies the `ftpk_` value.
  location: header
  name: Portal API key
  scopes:
  - seo
  - aeo
  - geo
  - smm
  - outreach
  - paid_media
  - plan
  - leads:mark
  type: http-bearer
- evidence: No credential / `Bearer demo`
  how_to_obtain: None – the public demo workspace is accessible without a credential.
  name: No credential / `Bearer demo`
  type: http-bearer
slug: fractionalteams-com-authentication
source_filename: fractionalteams-com-authentication.yml
source_heading: Authentication Profile
source_url: https://portal.fractionalteams.com/auth.md
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://portal.fractionalteams.com/auth.md\nsources:\n- https://portal.fractionalteams.com/auth.md\n- https://portal.fractionalteams.com/.well-known/oauth-protected-resource\ndescription: Authentication schemes for Fractional Teams Portal API\nschemes:\n- type: http-bearer\n  name: Portal API key\n  evidence: 'The portal uses **per-user bearer API keys**, not OAuth: there is no authorization server, no `agent_auth` endpoint and no dynamic\n    `register_uri`: a human issues the key.'\n  location: header\n  header: Authorization\n  scopes:\n  - seo\n  - aeo\n  - geo\n  - smm\n  - outreach\n  - paid_media\n  - plan\n  - leads:mark\n  how_to_obtain: Human creates the key on the portal account page (https://portal.fractionalteams.com/account) → API keys → Create key and copies\n    the `ftpk_` value.\n- type: http-bearer\n  name: No credential / `Bearer demo`\n  evidence: No credential\
  \ / `Bearer demo`\n  how_to_obtain: None – the public demo workspace is accessible without a credential.\ndocs: https://portal.fractionalteams.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/fractionalteams-com/authentication/fractionalteams-com-authentication.yml
summary_line: 2 schemes
tags:
- Marketing
- Product Consulting
- CxO Leadership
- Lead Generation
- Cloud Strategy
- Technical Platforms
- Event
---
