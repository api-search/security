---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gatecoreai-com-openapi-generated.yml
  format: yaml
  label: GateCore AI API
  slug: gatecoreai-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gatecoreai-com/openapi/_ae-authored/gatecoreai-com-openapi-generated.yml
auth_types: []
description: Authentication schemes for GateCore AI MCP API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: GateCore AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: GateCore AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GateCore AI
provider_slug: gatecoreai-com
scheme_count: 1
schemes:
- evidence: 'Use Authorization: Bearer <key> on each request.'
  header: Authorization
  how_to_obtain: Copy the gcmk_... MCP key when the portal reveals it.
  location: header
  name: Bearer
  type: http-bearer
slug: gatecoreai-com-authentication
source_filename: gatecoreai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://gatecoreai.com/quickstart/
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gatecoreai.com/quickstart/\nsources:\n- https://gatecoreai.com/quickstart/\ndescription: Authentication schemes for GateCore AI MCP API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Use Authorization: Bearer <key> on each request.'\n  location: header\n  header: Authorization\n  how_to_obtain: Copy the gcmk_... MCP key when the portal reveals it.\ndocs: https://gatecoreai.com/quickstart/\n"
source_yaml_url: https://artifacts.apis.io/gatecoreai-com/authentication/gatecoreai-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Platform
- Governance
- Marketplace
- Security
- Enterprise
---
