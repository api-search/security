---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Pantry Persona
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Pantry Persona Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pantry Persona declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Pantry Persona
provider_slug: pantrypersona-com
scheme_count: 1
schemes:
- authorize_url: /api/oauth/authorize
  evidence: Auth OAuth 2.0 with PKCE Authorization /api/oauth/authorize Token /api/oauth/token Scopes pantry, recipes, meal-plans, shopping, profiles
  flows:
  - authorization_code
  how_to_obtain: Most MCP clients handle OAuth automatically. You'll be prompted to sign in on first use.
  name: OAuth 2.0 with PKCE
  scopes:
  - pantry
  - recipes
  - meal-plans
  - shopping
  - profiles
  type: oauth2
slug: pantrypersona-com-authentication
source_filename: pantrypersona-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.pantrypersona.com/setup/developer
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.pantrypersona.com/setup/developer\nsources:\n- https://www.pantrypersona.com/setup/developer\n- https://www.pantrypersona.com/setup/home-assistant\n- https://www.pantrypersona.com/setup/openclaw\ndescription: Authentication methods for Pantry Persona\nschemes:\n- type: oauth2\n  name: OAuth 2.0 with PKCE\n  evidence: Auth OAuth 2.0 with PKCE Authorization /api/oauth/authorize Token /api/oauth/token Scopes pantry, recipes, meal-plans, shopping, profiles\n  flows:\n  - authorization_code\n  authorize_url: /api/oauth/authorize\n  scopes:\n  - pantry\n  - recipes\n  - meal-plans\n  - shopping\n  - profiles\n  how_to_obtain: Most MCP clients handle OAuth automatically. You'll be prompted to sign in on first use.\ndocs: https://www.pantrypersona.com/setup/developer\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/pantrypersona-com/authentication/pantrypersona-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Kitchen
- Pantry
- Meal Planning
- Software-as-a-Service
---
