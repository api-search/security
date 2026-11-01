---
anonymous_access: false
api_key_in: []
api_specs:
- filename: myopl-net-mcp-api-openapi.yml
  format: yaml
  label: myopl-net MCP API
  slug: myopl-net-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopl-net/openapi/myopl-net-mcp-api-openapi.yml
auth_types: []
description: Authentication methods described on the MYOPL auth pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Myopl Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: myopl-net declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: myopl-net
provider_slug: myopl-net
scheme_count: 2
schemes:
- evidence: Send the resulting access token only as an Authorization Bearer header to the personal endpoint.
  header: Authorization
  how_to_obtain: Use a published client identity or dynamic client registration, then authorization code with PKCE S256 and the exact registered callback.
  location: header
  name: OAuth2 Bearer
  scopes:
  - myopl:rating:read
  - myopl:sessions:read
  - myopl:rsvp:write
  - myopl:statistics:read
  type: http-bearer
- evidence: Requests require `X-AI-Client-ID`, `X-AI-Timestamp`, `X-AI-Nonce` and `X-AI-Signature` according to the signing instructions supplied when a client is provisioned.
  how_to_obtain: Manual approval and provisioning of a MYOPL signing client via the MYOPL Contact page.
  location: header
  name: A2A signing
  type: other
slug: myopl-net-authentication
source_filename: myopl-net-authentication.yml
source_heading: Authentication Profile
source_url: https://myopl.net/auth.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://myopl.net/auth.md\nsources:\n- https://myopl.net/auth.md\n- https://myopl.net/auth.es.md\ndescription: Authentication methods described on the MYOPL auth pages.\nschemes:\n- type: http-bearer\n  name: OAuth2 Bearer\n  evidence: Send the resulting access token only as an Authorization Bearer header to the personal endpoint.\n  location: header\n  header: Authorization\n  scopes:\n  - myopl:rating:read\n  - myopl:sessions:read\n  - myopl:rsvp:write\n  - myopl:statistics:read\n  how_to_obtain: Use a published client identity or dynamic client registration, then authorization code with PKCE S256 and the exact registered\n    callback.\n- type: other\n  name: A2A signing\n  evidence: Requests require `X-AI-Client-ID`, `X-AI-Timestamp`, `X-AI-Nonce` and `X-AI-Signature` according to the signing instructions supplied\n    when a client is provisioned.\n  location: header\n  how_to_obtain:\
  \ Manual approval and provisioning of a MYOPL signing client via the MYOPL Contact page.\nnote: Public reference access requires no authentication.\ndocs: https://myopl.net/auth.md\n"
source_yaml_url: https://artifacts.apis.io/myopl-net/authentication/myopl-net-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Pickleball
- Sports
- Community
- Platform
---
