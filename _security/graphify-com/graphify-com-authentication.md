---
anonymous_access: false
api_key_in: []
api_specs:
- filename: graphify-com-openapi-generated.yml
  format: yaml
  label: Graphify API
  slug: graphify-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/graphify-com/openapi/_ae-authored/graphify-com-openapi-generated.yml
auth_types: []
description: Authentication for Graphify’s hosted MCP server uses OAuth.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Graphify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Graphify declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Graphify
provider_slug: graphify-com
scheme_count: 1
schemes:
- evidence: 'Graphify is the hosted product: https://api.graphify.com/mcp (Streamable HTTP, OAuth, no API key).'
  how_to_obtain: The first connection opens an OAuth sign-in. There is no API key to paste.
  name: Graphify OAuth
  type: oauth2
slug: graphify-com-authentication
source_filename: graphify-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.graphify.com/open-source/features/token-benchmark.md
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.graphify.com/open-source/features/token-benchmark.md\nsources:\n- https://docs.graphify.com/open-source/features/token-benchmark.md\n- https://docs.graphify.com/open-source/features/honest-token-savings.md\n- https://docs.graphify.com/platform/quickstart.md\n- https://docs.graphify.com/open-source/quickstart.md\ndescription: Authentication for Graphify’s hosted MCP server uses OAuth.\nschemes:\n- type: oauth2\n  name: Graphify OAuth\n  evidence: 'Graphify is the hosted product: https://api.graphify.com/mcp (Streamable HTTP, OAuth, no API key).'\n  how_to_obtain: The first connection opens an OAuth sign-in. There is no API key to paste.\ndocs: https://docs.graphify.com/open-source/features/token-benchmark.md\n"
source_yaml_url: https://artifacts.apis.io/graphify-com/authentication/graphify-com-authentication.yml
summary_line: 1 scheme
tags:
- code graph
- Developer Tools
- Source Code Analysis
- Pull Request Review
- Open Source
- Hosted Service
---
