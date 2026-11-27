---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ironflow-sh-hyperliquid-api-openapi.yml
  format: yaml
  label: Ironflow Hyperliquid API
  slug: ironflow-sh-hyperliquid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ironflow-sh/openapi/ironflow-sh-hyperliquid-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ironflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ironflow declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ironflow
provider_slug: ironflow-sh
scheme_count: 1
schemes:
- evidence: Send a key in the `Authorization` header for more history and a higher rate limit.
  header: Authorization
  how_to_obtain: Get a free key at https://ironflow.sh/key or request one via POST /v1/keys
  location: header
  name: Bearer
  type: http-bearer
slug: ironflow-sh-authentication
source_filename: ironflow-sh-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ironflow.sh/authentication.md
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ironflow.sh/authentication.md\nsources:\n- https://docs.ironflow.sh/authentication.md\n- https://docs.ironflow.sh/guides/hyperliquid-rpc.md\n- https://docs.ironflow.sh/api-reference/billing/request-key.md\n- https://docs.ironflow.sh/api-reference/billing/request-upgrade.md\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Send a key in the `Authorization` header for more history and a higher rate limit.\n  location: header\n  header: Authorization\n  how_to_obtain: Get a free key at https://ironflow.sh/key or request one via POST /v1/keys\ndocs: https://docs.ironflow.sh/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/ironflow-sh/authentication/ironflow-sh-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data API
- Trading
- Sandbox
- Hyperliquid
- MCP
---
