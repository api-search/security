---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Cofferline API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cofferline Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cofferline declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cofferline
provider_slug: cofferline-com
scheme_count: 1
schemes:
- evidence: 'Example curl -X GET https://api.cofferline.com/v1/keys \ -H "authorization: Bearer $TOKEN"'
  header: Authorization
  how_to_obtain: Obtain a session token via SIWE authentication (POST /v1/auth/verify) or create an API key via POST /v1/keys; the token is returned once and used as a Bearer token.
  location: header
  name: Bearer token
  type: http-bearer
slug: cofferline-com-authentication
source_filename: cofferline-com-authentication.yml
source_heading: Authentication Profile
source_url: https://cofferline.com/docs/api/keys
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cofferline.com/docs/api/keys\nsources:\n- https://cofferline.com/docs/api/keys\n- https://cofferline.com/docs/api/auth\n- https://cofferline.com/docs/api/tokens\n- https://cofferline.com/docs/agent-quickstart\ndescription: Authentication methods for Cofferline API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Example curl -X GET https://api.cofferline.com/v1/keys \\ -H \"authorization: Bearer $TOKEN\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a session token via SIWE authentication (POST /v1/auth/verify) or create an API key via POST /v1/keys; the token is returned\n    once and used as a Bearer token.\ndocs: https://cofferline.com/docs/api/keys\n"
source_yaml_url: https://artifacts.apis.io/cofferline-com/authentication/cofferline-com-authentication.yml
summary_line: 1 scheme
tags:
- Treasury
- Prediction Markets
- Non-Custodial
- SIWE Authentication
- Agent Infrastructure
---
