---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clearpolicy-app-api-openapi.json
  format: json
  label: ClearPolicy API API
  slug: clearpolicy-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearpolicy-app/openapi/_original/clearpolicy-app-api-openapi.json
auth_types: []
description: Authentication methods for ClearPolicy API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ClearPolicy Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClearPolicy declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ClearPolicy
provider_slug: clearpolicy-app
scheme_count: 1
schemes:
- evidence: The REST API uses **API tokens** sent as bearer tokens.
  header: Authorization
  how_to_obtain: Create an API token via Settings → API, give it a name, and copy the token when shown.
  location: header
  name: API token
  type: http-bearer
slug: clearpolicy-app-authentication
source_filename: clearpolicy-app-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.clearpolicy.app/api/authentication.md
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.clearpolicy.app/api/authentication.md\nsources:\n- https://docs.clearpolicy.app/api/authentication.md\n- https://docs.clearpolicy.app/guides/signer-portal.md\n- https://docs.clearpolicy.app/guides/signing-help.md\n- https://docs.clearpolicy.app/quickstart.md\ndescription: Authentication methods for ClearPolicy API\nschemes:\n- type: http-bearer\n  name: API token\n  evidence: The REST API uses **API tokens** sent as bearer tokens.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API token via Settings → API, give it a name, and copy the token when shown.\ndocs: https://docs.clearpolicy.app/api/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/clearpolicy-app/authentication/clearpolicy-app-authentication.yml
summary_line: 1 scheme
tags:
- Policy
- E-Signature
- Software-as-a-Service
- Small Business
- Non-Profit
---
