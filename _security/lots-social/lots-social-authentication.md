---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lots-social-openapi-generated.yml
  format: yaml
  label: LotsSocial API
  slug: lots-social-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lots-social/openapi/_ae-authored/lots-social-openapi-generated.yml
auth_types: []
description: Authentication methods for LotsSocial as described on the documentation pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LotsSocial Authentication
name_suffix: Authentication
oauth_flows: []
overview: LotsSocial declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LotsSocial
provider_slug: lots-social
scheme_count: 2
schemes:
- evidence: 'Agents that only accept a header can send `Authorization: Bearer <API key>`, with a key from https://www.lotstech.com/api.'
  header: Authorization
  how_to_obtain: Obtain an API key from https://www.lotstech.com/api.
  location: header
  name: Bearer
  type: http-bearer
- evidence: Enter the LotsSocial connection. Name it LotsSocial. Under Connection, enter the server URL below, then choose OAuth for authentication.
  name: OAuth
  type: oauth2
slug: lots-social-authentication
source_filename: lots-social-authentication.yml
source_heading: Authentication Profile
source_url: https://lots.social/agents.md
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lots.social/agents.md\nsources:\n- https://lots.social/agents.md\ndescription: Authentication methods for LotsSocial as described on the documentation pages.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Agents that only accept a header can send `Authorization: Bearer <API key>`, with a key from https://www.lotstech.com/api.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain an API key from https://www.lotstech.com/api.\n- type: oauth2\n  name: OAuth\n  evidence: Enter the LotsSocial connection. Name it LotsSocial. Under Connection, enter the server URL below, then choose OAuth for authentication.\ndocs: https://lots.social/agents.md\n"
source_yaml_url: https://artifacts.apis.io/lots-social/authentication/lots-social-authentication.yml
summary_line: 2 schemes
tags:
- Social Media Scheduler
- AI Integration
---
