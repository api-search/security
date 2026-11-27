---
anonymous_access: false
api_key_in: []
api_specs:
- filename: makepartsnow-com-agent-api-openapi.yml
  format: yaml
  label: Make Parts Now Agent API
  slug: makepartsnow-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makepartsnow-com/openapi/makepartsnow-com-agent-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Make Parts Now Authentication
name_suffix: Authentication
oauth_flows: []
overview: Make Parts Now declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Make Parts Now
provider_slug: makepartsnow-com
scheme_count: 2
schemes:
- evidence: Sign in with your website account (OAuth) Add the server, and your client opens a sign-in page.
  name: OAuth
  type: oauth2
- evidence: For an agent with no person behind it, create an agent account and send its key as a Bearer token.
  header: Authorization
  how_to_obtain: Create an agent account to obtain the token.
  location: header
  name: Bearer token
  type: http-bearer
slug: makepartsnow-com-authentication
source_filename: makepartsnow-com-authentication.yml
source_heading: Authentication Profile
source_url: https://makepartsnow.com/developers#ai-assistants
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://makepartsnow.com/developers#ai-assistants\nsources:\n- https://makepartsnow.com/developers#ai-assistants\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Sign in with your website account (OAuth) Add the server, and your client opens a sign-in page.\n- type: http-bearer\n  name: Bearer token\n  evidence: For an agent with no person behind it, create an agent account and send its key as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an agent account to obtain the token.\ndocs: https://makepartsnow.com/developers#ai-assistants\n"
source_yaml_url: https://artifacts.apis.io/makepartsnow-com/authentication/makepartsnow-com-authentication.yml
summary_line: 2 schemes
tags:
- Manufacturing
- 3D Printing
- CNC Machining
- Custom Parts
- E-Commerce
---
