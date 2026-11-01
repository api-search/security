---
anonymous_access: false
api_key_in: []
api_specs:
- filename: netmon-com-openapi-generated.yml
  format: yaml
  label: netmon-com API
  slug: netmon-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netmon-com/openapi/_ae-authored/netmon-com-openapi-generated.yml
auth_types: []
description: Authentication schemes for Netmon API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Netmon Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: netmon-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: netmon-com
provider_slug: netmon-com
scheme_count: 1
schemes:
- evidence: Every call to the Netmon REST API is made on behalf of a user, and every call carries a bearer token in the `Authorization` header.
  header: Authorization
  how_to_obtain: 'Three credential types resolve to a bearer token: a session token from POST /api/login, a personal access token minted via POST /api/tokens, or an OAuth token obtained through a browser sign‑in flow.'
  location: header
  name: Bearer token
  type: http-bearer
slug: netmon-com-authentication
source_filename: netmon-com-authentication.yml
source_heading: Authentication Profile
source_url: https://netmon.com/wp-content/uploads/2026/08/netmon-docs-api-authentication.txt
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://netmon.com/wp-content/uploads/2026/08/netmon-docs-api-authentication.txt\nsources:\n- https://netmon.com/wp-content/uploads/2026/08/netmon-docs-api-authentication.txt\ndescription: Authentication schemes for Netmon API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Every call to the Netmon REST API is made on behalf of a user, and every call carries a bearer token in the `Authorization` header.\n  location: header\n  header: Authorization\n  how_to_obtain: 'Three credential types resolve to a bearer token: a session token from POST /api/login, a personal access token minted via POST\n    /api/tokens, or an OAuth token obtained through a browser sign‑in flow.'\nnote: OAuth flow URLs, specific scopes, and detailed OAuth flow types are not provided on the page.\ndocs: https://netmon.com/wp-content/uploads/2026/08/netmon-docs-api-authentication.txt\n"
source_yaml_url: https://artifacts.apis.io/netmon-com/authentication/netmon-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Network Monitoring
- Self-Hosted
- AI Integration
- Open Source
---
