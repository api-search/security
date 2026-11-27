---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jsonify-com-openapi-generated.yml
  format: yaml
  label: Jsonify API
  slug: jsonify-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jsonify-com/openapi/_ae-authored/jsonify-com-openapi-generated.yml
auth_types: []
description: Authentication for Jsonify MCP API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Jsonify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jsonify declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Jsonify
provider_slug: jsonify-com
scheme_count: 1
schemes:
- evidence: Use the resulting bearer access token with the MCP endpoint at that resource.
  header: Authorization
  how_to_obtain: Obtain an identity assertion via the registration endpoint (service_auth or anonymous), optionally complete a claim ceremony, then exchange the assertion for an access token using the JWT‑bearer grant at the token URL.
  location: header
  name: Bearer
  token_url: https://auth.jsonify.com/oauth2/token
  type: http-bearer
slug: jsonify-com-authentication
source_filename: jsonify-com-authentication.yml
source_heading: Authentication Profile
source_url: https://factory.jsonify.com/auth.md
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://factory.jsonify.com/auth.md\nsources:\n- https://factory.jsonify.com/auth.md\n- https://www.jsonify.com/docs/getting-started/first-pipeline.md\n- https://www.jsonify.com/docs/getting-started/glossary.md\n- https://www.jsonify.com/docs/getting-started/workspaces.md\ndescription: Authentication for Jsonify MCP API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Use the resulting bearer access token with the MCP endpoint at that resource.\n  location: header\n  header: Authorization\n  token_url: https://auth.jsonify.com/oauth2/token\n  how_to_obtain: Obtain an identity assertion via the registration endpoint (service_auth or anonymous), optionally complete a claim ceremony,\n    then exchange the assertion for an access token using the JWT‑bearer grant at the token URL.\ndocs: https://factory.jsonify.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/jsonify-com/authentication/jsonify-com-authentication.yml
summary_line: 1 scheme
tags:
- Data
- Artificial Intelligence
- Automation
- Datasets
- Software-as-a-Service
---
