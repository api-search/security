---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ogenhq-com-rest-api-openapi.yml
  format: yaml
  label: Ogen Rest API
  slug: ogenhq-com-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogenhq-com/openapi/ogenhq-com-rest-api-openapi.yml
auth_types: []
description: Authentication schemes for Ogen as documented on the Quick Start page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ogen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ogen declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ogen
provider_slug: ogenhq-com
scheme_count: 1
schemes:
- evidence: 'Point any MCP client at Ogen: no SDK, no local code. No key yet? Get a free key.'
  header: Authorization
  how_to_obtain: Obtain a free key from the Ogen site or use the OAuth sign‑in flow.
  location: header
  name: Bearer token
  type: http-bearer
slug: ogenhq-com-authentication
source_filename: ogenhq-com-authentication.yml
source_heading: Authentication Profile
source_url: https://ogenhq.com/docs/quick-start
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ogenhq.com/docs/quick-start\nsources:\n- https://ogenhq.com/docs/quick-start\ndescription: Authentication schemes for Ogen as documented on the Quick Start page.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Point any MCP client at Ogen: no SDK, no local code. No key yet? Get a free key.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a free key from the Ogen site or use the OAuth sign‑in flow.\nnote: The page mentions an OAuth flow for sign‑in but does not provide token or authorize URLs or scopes, so those fields are left null/empty.\ndocs: https://ogenhq.com/docs/quick-start\n"
source_yaml_url: https://artifacts.apis.io/ogenhq-com/authentication/ogenhq-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Automation
- Workflows
- Compliance
- Data Integration
---
