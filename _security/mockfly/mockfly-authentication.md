---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mockfly-openapi.json
  format: json
  label: Mockfly Public API
  slug: mockfly-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mockfly/openapi/mockfly-openapi.json
auth_types: []
description: Mockfly uses an account API key for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mockfly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mockfly declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mockfly
provider_slug: mockfly
scheme_count: 1
schemes:
- evidence: To add endpoints with the chrome extension or the public API , use an account API key from app.mockfly.dev/api-keys .
  header: Authorization
  how_to_obtain: Generate an API key in the Mockfly dashboard at app.mockfly.dev/api-keys.
  location: header
  name: Account API Key
  type: apiKey
slug: mockfly-authentication
source_filename: mockfly-authentication.yml
source_heading: Authentication Profile
source_url: https://mockfly.dev/docs/
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mockfly.dev/docs/\nsources:\n- https://mockfly.dev/docs/\n- https://mockfly.dev/articles/getting-started-with-mockfly/\n- https://mockfly.dev/docs\ndescription: Mockfly uses an account API key for authentication.\nschemes:\n- type: apiKey\n  name: Account API Key\n  evidence: To add endpoints with the chrome extension or the public API , use an account API key from app.mockfly.dev/api-keys .\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the Mockfly dashboard at app.mockfly.dev/api-keys.\ndocs: https://mockfly.dev/docs/\n"
source_yaml_url: https://artifacts.apis.io/mockfly/authentication/mockfly-authentication.yml
summary_line: 1 scheme
tags:
- API Platform
- Mock APIs
- Developer Tools
- Testing
- CI/CD Integration
---
