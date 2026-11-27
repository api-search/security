---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tallyworkout-app-openapi-generated.yml
  format: yaml
  label: Tally Workout API
  slug: tallyworkout-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tallyworkout-app/openapi/_ae-authored/tallyworkout-app-openapi-generated.yml
auth_types: []
description: Tally Workout uses a simple API key that is sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Tally Workout Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tally Workout declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Tally Workout
provider_slug: tallyworkout-app
scheme_count: 1
schemes:
- evidence: http_headers = { "Authorization" = "Bearer your-key" }
  header: Authorization
  how_to_obtain: Create a key in the Tally app under Settings → API keys → Create key, then copy the displayed key.
  location: header
  name: Bearer
  type: http-bearer
slug: tallyworkout-app-authentication
source_filename: tallyworkout-app-authentication.yml
source_heading: Authentication Profile
source_url: https://tallyworkout.app/connect/codex
source_yaml: "generated: '2026-11-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://tallyworkout.app/connect/codex\nsources:\n- https://tallyworkout.app/connect/codex\n- https://tallyworkout.app/connect/hark\n- https://tallyworkout.app/connect/dots\n- https://tallyworkout.app/connect/perplexity\ndescription: Tally Workout uses a simple API key that is sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: http_headers = { \"Authorization\" = \"Bearer your-key\" }\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the Tally app under Settings → API keys → Create key, then copy the displayed key.\ndocs: https://tallyworkout.app/connect/codex\n"
source_yaml_url: https://artifacts.apis.io/tallyworkout-app/authentication/tallyworkout-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Fitness
- AI
- Mobile
- Workout
- Health
---
