---
anonymous_access: false
api_key_in: []
api_specs:
- filename: opsmeter-openapi-generated.yml
  format: yaml
  label: Opsmeter.io API
  slug: opsmeter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opsmeter/openapi/_ae-authored/opsmeter-openapi-generated.yml
auth_types: []
description: Opsmeter.io uses a workspace API key for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Opsmeter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opsmeter.io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Opsmeter.io
provider_slug: opsmeter
scheme_count: 1
schemes:
- evidence: Generate a workspace API key After sign-in, rotate a new key in Settings → API keys . Keys are shown only once. Then continue with a ready payload and send your first ingest call.
  header: X-API-Key
  how_to_obtain: Create a workspace API key in Settings → API keys after signing in.
  location: header
  name: X-API-Key
  type: apiKey
slug: opsmeter-authentication
source_filename: opsmeter-authentication.yml
source_heading: Authentication Profile
source_url: https://opsmeter.io/docs/quickstart
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://opsmeter.io/docs/quickstart\nsources:\n- https://opsmeter.io/docs/quickstart\ndescription: Opsmeter.io uses a workspace API key for authentication.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Generate a workspace API key After sign-in, rotate a new key in Settings → API keys . Keys are shown only once. Then continue with\n    a ready payload and send your first ingest call.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a workspace API key in Settings → API keys after signing in.\nnote: No other authentication schemes (OAuth, HTTP basic, etc.) are documented on the page.\ndocs: https://opsmeter.io/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/opsmeter/authentication/opsmeter-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Cost Management
- Monitoring
- Observability
---
