---
anonymous_access: false
api_key_in: []
api_specs:
- filename: scavio-openapi-generated.yml
  format: yaml
  label: Scavio API
  slug: scavio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scavio/openapi/_ae-authored/scavio-openapi-generated.yml
auth_types: []
description: Scavio uses a simple API key presented as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Scavio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scavio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Scavio
provider_slug: scavio
scheme_count: 1
schemes:
- evidence: 'headers = { "Authorization" : f "Bearer {API_KEY}" }'
  header: Authorization
  how_to_obtain: Obtain an API key from the Scavio Dashboard (API Keys page).
  location: header
  name: Bearer
  type: http-bearer
slug: scavio-authentication
source_filename: scavio-authentication.yml
source_heading: Authentication Profile
source_url: https://scavio.dev/solutions/reddit-data-without-api-key
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://scavio.dev/solutions/reddit-data-without-api-key\nsources:\n- https://scavio.dev/solutions/reddit-data-without-api-key\n- https://scavio.dev/best/best-agent-token-reduction-tools-2026\n- https://scavio.dev/docs/quickstart\n- https://scavio.dev/docs/python-sdk-quickstart\ndescription: Scavio uses a simple API key presented as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'headers = { \"Authorization\" : f \"Bearer {API_KEY}\" }'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain an API key from the Scavio Dashboard (API Keys page).\ndocs: https://scavio.dev/solutions/reddit-data-without-api-key\n"
source_yaml_url: https://artifacts.apis.io/scavio/authentication/scavio-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Web Scraping
- Data
- Artificial Intelligence
---
