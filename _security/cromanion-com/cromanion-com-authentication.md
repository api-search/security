---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cromanion-com-openapi-generated.yml
  format: yaml
  label: Cromanion API
  slug: cromanion-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cromanion-com/openapi/_ae-authored/cromanion-com-openapi-generated.yml
auth_types: []
description: Cromanion authenticates to HubSpot using OAuth. The user clicks Connect HubSpot, is sent to HubSpot's consent screen, approves scopes, and HubSpot returns a token that Cromanion stores server‑side.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cromanion Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cromanion declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cromanion
provider_slug: cromanion-com
scheme_count: 1
schemes:
- evidence: Cromanion never sees your HubSpot password; it receives a token from HubSpot after you approve, and that token is stored server-side and never sent to a browser.
  flows:
  - authorization_code
  how_to_obtain: User clicks Connect HubSpot, is redirected to HubSpot's consent screen, approves requested scopes, and HubSpot returns an access token to Cromanion.
  name: HubSpot OAuth
  scopes:
  - oauth
  - crm.objects.contacts.write
  type: oauth2
slug: cromanion-com-authentication
source_filename: cromanion-com-authentication.yml
source_heading: Authentication Profile
source_url: https://cromanion.com/hubspot/setup
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cromanion.com/hubspot/setup\nsources:\n- https://cromanion.com/hubspot/setup\ndescription: Cromanion authenticates to HubSpot using OAuth. The user clicks Connect HubSpot, is sent to HubSpot's consent screen, approves scopes,\n  and HubSpot returns a token that Cromanion stores server‑side.\nschemes:\n- type: oauth2\n  name: HubSpot OAuth\n  evidence: Cromanion never sees your HubSpot password; it receives a token from HubSpot after you approve, and that token is stored server-side\n    and never sent to a browser.\n  flows:\n  - authorization_code\n  scopes:\n  - oauth\n  - crm.objects.contacts.write\n  how_to_obtain: User clicks Connect HubSpot, is redirected to HubSpot's consent screen, approves requested scopes, and HubSpot returns an access\n    token to Cromanion.\ndocs: https://cromanion.com/hubspot/setup\n"
source_yaml_url: https://artifacts.apis.io/cromanion-com/authentication/cromanion-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- CRO
- Conversion
- Marketing
- Software-as-a-Service
---
