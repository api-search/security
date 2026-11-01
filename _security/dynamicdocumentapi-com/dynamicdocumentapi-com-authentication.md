---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Dynamic Document API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dynamicdocumentapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dynamic Document API declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Dynamic Document API
provider_slug: dynamicdocumentapi-com
scheme_count: 2
schemes:
- evidence: 'Pass the key as a bearer token in the `Authorization` header:'
  header: Authorization
  location: header
  name: Authorization Bearer
  type: http-bearer
- evidence: 'Tools that can only set a custom header can send the key in `X-API-Key` instead:'
  header: X-API-Key
  location: header
  name: X-API-Key
  type: apiKey
slug: dynamicdocumentapi-com-authentication
source_filename: dynamicdocumentapi-com-authentication.yml
source_heading: Authentication Profile
source_url: https://dynamicdocumentapi.com/docs/authentication/index.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dynamicdocumentapi.com/docs/authentication/index.md\nsources:\n- https://dynamicdocumentapi.com/docs/authentication/index.md\n- https://dynamicdocumentapi.com/docs/authentication\n- https://dynamicdocumentapi.com/docs/quickstart\n- https://dynamicdocumentapi.com/docs/quickstart/index.md\ndescription: Authentication schemes for Dynamic Document API\nschemes:\n- type: http-bearer\n  name: Authorization Bearer\n  evidence: 'Pass the key as a bearer token in the `Authorization` header:'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Tools that can only set a custom header can send the key in `X-API-Key` instead:'\n  location: header\n  header: X-API-Key\nnote: OAuth flows are mentioned (Zapier, Make, MCP server) but no token or authorize URLs are provided, so OAuth details are absent.\ndocs: https://dynamicdocumentapi.com/docs/authentication/index.md\n"
source_yaml_url: https://artifacts.apis.io/dynamicdocumentapi-com/authentication/dynamicdocumentapi-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- PDF
- Image Generation
- E-invoicing
- REST API
---
