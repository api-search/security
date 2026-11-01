---
anonymous_access: false
api_key_in: []
api_specs:
- filename: runcrate-api-openapi.json
  format: json
  label: Runcrate API API
  slug: runcrate-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/runcrate/openapi/_original/runcrate-api-openapi.json
auth_types: []
description: Runcrate API authentication uses API keys passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Runcrate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Runcrate declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Runcrate
provider_slug: runcrate
scheme_count: 1
schemes:
- evidence: All API requests require a Runcrate API key passed as a Bearer token.
  header: Authorization
  how_to_obtain: Create an API key in the Dashboard → Keys page; the full key is shown once and can be copied.
  location: header
  name: Runcrate API Key
  type: http-bearer
slug: runcrate-authentication
source_filename: runcrate-authentication.yml
source_heading: Authentication Profile
source_url: https://www.runcrate.ai/docs/account/api-keys
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.runcrate.ai/docs/account/api-keys\nsources:\n- https://www.runcrate.ai/docs/account/api-keys\n- https://www.runcrate.ai/docs/models/authentication\n- https://www.runcrate.ai/docs/account/authentication\ndescription: Runcrate API authentication uses API keys passed as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Runcrate API Key\n  evidence: All API requests require a Runcrate API key passed as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the Dashboard → Keys page; the full key is shown once and can be copied.\ndocs: https://www.runcrate.ai/docs/account/api-keys\n"
source_yaml_url: https://artifacts.apis.io/runcrate/authentication/runcrate-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- GPU
- Inference
- Compute
- Platform
---
