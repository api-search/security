---
anonymous_access: false
api_key_in: []
api_specs:
- filename: browserforest-com-openapi-generated.yml
  format: yaml
  label: Browser Forest API
  slug: browserforest-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/browserforest-com/openapi/_ae-authored/browserforest-com-openapi-generated.yml
auth_types: []
description: Browser Forest uses API Key authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Browserforest Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Browser Forest declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Browser Forest
provider_slug: browserforest-com
scheme_count: 1
schemes:
- evidence: Browser Forest uses API Key authentication. Include your key via the X-API-Key header on every request.
  header: X-API-Key
  how_to_obtain: Create an API Key via POST /v1/auth/api-keys (returns a key starting with bf_live_).
  location: header
  name: X-API-Key
  type: apiKey
slug: browserforest-com-authentication
source_filename: browserforest-com-authentication.yml
source_heading: Authentication Profile
source_url: https://browserforest.com/docs/authentication
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://browserforest.com/docs/authentication\nsources:\n- https://browserforest.com/docs/authentication\n- https://browserforest.com/api/docs\n- https://browserforest.com/docs\ndescription: Browser Forest uses API Key authentication.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Browser Forest uses API Key authentication. Include your key via the X-API-Key header on every request.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an API Key via POST /v1/auth/api-keys (returns a key starting with bf_live_).\nnote: No OAuth2 or other authentication schemes are documented on the provided pages.\ndocs: https://browserforest.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/browserforest-com/authentication/browserforest-com-authentication.yml
summary_line: 1 scheme
tags:
- Cloud Browser
- AI Agents
- Automation
- Chromium
- Free Tier
---
