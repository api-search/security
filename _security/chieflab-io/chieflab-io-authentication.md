---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chieflab-io-connectors-api-openapi.yml
  format: yaml
  label: ChiefLab Connectors API
  slug: chieflab-io-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chieflab-io/openapi/chieflab-io-connectors-api-openapi.yml
- filename: chieflab-io-gtm-api-openapi.yml
  format: yaml
  label: ChiefLab GTM API
  slug: chieflab-io-gtm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chieflab-io/openapi/chieflab-io-gtm-api-openapi.yml
- filename: chieflab-io-mcp-api-openapi.yml
  format: yaml
  label: ChiefLab MCP API
  slug: chieflab-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chieflab-io/openapi/chieflab-io-mcp-api-openapi.yml
- filename: chieflab-io-public-api-openapi.yml
  format: yaml
  label: ChiefLab Public API
  slug: chieflab-io-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chieflab-io/openapi/chieflab-io-public-api-openapi.yml
- filename: chieflab-io-runs-api-openapi.yml
  format: yaml
  label: ChiefLab Runs API
  slug: chieflab-io-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chieflab-io/openapi/chieflab-io-runs-api-openapi.yml
- filename: chieflab-io-workspace-api-openapi.yml
  format: yaml
  label: ChiefLab Workspace API
  slug: chieflab-io-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chieflab-io/openapi/chieflab-io-workspace-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ChiefLab Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChiefLab secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ChiefLab
provider_slug: chieflab-io
scheme_count: 1
schemes:
- description: ChiefLab API key in the form `clp_dev_<key>` or `clp_live_<key>`. Mint one at https://chieflab.io/get-key (no email required for sandbox keys) or via the public `chieflab_signup_workspace` MCP tool.
  docs_text: Bearer token in the Authorization header. Keys start with clp_dev_ (dev/test) or clp_live_ (production).
  header: Authorization
  in: header
  key_prefixes:
  - mode: dev/test
    prefix: clp_dev_
  - mode: production
    prefix: clp_live_
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/chieflab-io-openapi.yml
  - https://chieflab.io/docs/mcp-reference
  type: http
slug: chieflab-io-authentication
source_filename: chieflab-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://chieflab.io/docs/mcp-reference\ndocs: https://chieflab.io/docs/mcp-reference\ndocs_pages:\n- https://chieflab.io/docs/mcp-reference\n- https://chieflab.io/docs/quickstart\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: ChiefLab API key in the form `clp_dev_<key>` or `clp_live_<key>`. Mint one at\n    https://chieflab.io/get-key (no email required for sandbox keys) or via the public `chieflab_signup_workspace`\n    MCP tool.\n  key_prefixes:\n  - prefix: clp_dev_\n    mode: dev/test\n  - prefix: clp_live_\n    mode: production\n  docs_text: \"Bearer token in the Authorization header. Keys start with clp_dev_ (dev/test) or clp_live_ (production).\"\n  sources:\n  - openapi/chieflab-io-openapi.yml\n  - https://chieflab.io/docs/mcp-reference\nunauthenticated_surfaces:\n- GET /api/mcp — endpoint metadata\n- tools/call for chieflab_signup_workspace\
  \ — agent-first signup, IP rate-limited (5 signups/IP/hour)\n- tools/call for chieflab_list_connectors — public connector registry (metadata only)\n- POST /api/sandbox/launch — no auth required, rate-limited to 3 calls per hour per IP (per /pricing FAQ)\nnote: Docs state \"Everything else requires a Bearer key.\" Trust page states API keys are SHA-256 hashed before persistence. Connector OAuth (GA4, Search Console, Zernio, Resend, HubSpot) is outbound to third parties, not an OAuth scheme on the ChiefLab API itself.\n"
source_yaml_url: https://artifacts.apis.io/chieflab-io/authentication/chieflab-io-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Agents
- Growth Marketing
- MCP
- Product Launch
- Marketing Automation
- Approval Workflows
- Developer Tools
---
