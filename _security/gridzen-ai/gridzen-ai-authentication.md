---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gridzen-ai-health-api-openapi.yml
  format: yaml
  label: gridzen-ai Health API
  slug: gridzen-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridzen-ai/openapi/gridzen-ai-health-api-openapi.yml
- filename: gridzen-ai-trust-decisions-api-openapi.yml
  format: yaml
  label: gridzen-ai Trust Decisions API
  slug: gridzen-ai-trust-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridzen-ai/openapi/gridzen-ai-trust-decisions-api-openapi.yml
auth_types: []
description: Authentication schemes as published on GridZen documentation pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Gridzen Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: gridzen-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: gridzen-ai
provider_slug: gridzen-ai
scheme_count: 1
schemes:
- evidence: Development authentication depends on your local configuration; when a decision key is configured, include X-API-Key.
  header: X-API-Key
  location: header
  name: X-API-Key
  type: apiKey
slug: gridzen-ai-authentication
source_filename: gridzen-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://gridzen.ai/developers/quickstart.html
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gridzen.ai/developers/quickstart.html\nsources:\n- https://gridzen.ai/developers/quickstart.html\n- https://gridzen.ai/docs/quickstart/\n- https://gridzen.ai/es/docs/quickstart/\n- https://gridzen.ai/zh/docs/quickstart/\ndescription: Authentication schemes as published on GridZen documentation pages.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Development authentication depends on your local configuration; when a decision key is configured, include X-API-Key.\n  location: header\n  header: X-API-Key\nnote: No OAuth2, HTTP Bearer, HTTP Basic, JWT, HMAC, mTLS, or other authentication schemes are documented.\ndocs: https://gridzen.ai/developers/quickstart.html\n"
source_yaml_url: https://artifacts.apis.io/gridzen-ai/authentication/gridzen-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Energy
- Grid
- Optimization
---
