---
anonymous_access: false
api_key_in: []
api_specs:
- filename: orvio-design-openapi-generated.yml
  format: yaml
  label: Orvio API
  slug: orvio-design-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orvio-design/openapi/_ae-authored/orvio-design-openapi-generated.yml
auth_types: []
description: Orvio uses OAuth 2.0 bearer token authentication sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Orvio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orvio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Orvio
provider_slug: orvio-design
scheme_count: 1
schemes:
- evidence: '"bearer_methods_supported":["header"]"'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: orvio-design-authentication
source_filename: orvio-design-authentication.yml
source_heading: Authentication Profile
source_url: https://mcp.orvio.design/.well-known/oauth-protected-resource/mcp
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mcp.orvio.design/.well-known/oauth-protected-resource/mcp\nsources:\n- https://mcp.orvio.design/.well-known/oauth-protected-resource/mcp\n- https://orvio.design/docs/products/design-tokens\n- https://orvio.design/docs/mcp/tools/read_tokens\n- https://orvio.design/docs/mcp/identifiers\ndescription: Orvio uses OAuth 2.0 bearer token authentication sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '\"bearer_methods_supported\":[\"header\"]\"'\n  location: header\n  header: Authorization\ndocs: https://mcp.orvio.design/.well-known/oauth-protected-resource/mcp\n"
source_yaml_url: https://artifacts.apis.io/orvio-design/authentication/orvio-design-authentication.yml
summary_line: 1 scheme
tags:
- Design
- UI
- Catalog
- Web
---
