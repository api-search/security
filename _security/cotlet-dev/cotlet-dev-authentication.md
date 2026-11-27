---
anonymous_access: false
api_key_in: []
auth_types: []
description: Cotlet API authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cotlet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cotlet declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cotlet
provider_slug: cotlet-dev
scheme_count: 1
schemes:
- evidence: Every call carries your API key as a bearer token.
  header: Authorization
  how_to_obtain: Create an API key in the Cotlet dashboard (console).
  location: header
  name: Bearer
  type: http-bearer
slug: cotlet-dev-authentication
source_filename: cotlet-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://cotlet.dev/docs
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cotlet.dev/docs\nsources:\n- https://cotlet.dev/docs\ndescription: Cotlet API authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Every call carries your API key as a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the Cotlet dashboard (console).\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the page.\ndocs: https://cotlet.dev/docs\n"
source_yaml_url: https://artifacts.apis.io/cotlet-dev/authentication/cotlet-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Automation
- Artificial Intelligence
- Integration
---
