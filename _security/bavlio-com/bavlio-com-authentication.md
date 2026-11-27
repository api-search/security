---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Bavlio API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bavlio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bavlio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bavlio
provider_slug: bavlio-com
scheme_count: 1
schemes:
- evidence: Bearer authentication header of the form Bearer <token> , where <token> is your auth token.
  header: Authorization
  how_to_obtain: Create an API key via POST /api-keys (or receive a sign‑in token after registration) and use the returned secret as the Bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: bavlio-com-authentication
source_filename: bavlio-com-authentication.yml
source_heading: Authentication Profile
source_url: https://bavlio.com/docs/api-reference/auth/list-api-keys
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://bavlio.com/docs/api-reference/auth/list-api-keys\nsources:\n- https://bavlio.com/docs/api-reference/auth/list-api-keys\n- https://bavlio.com/docs/api-reference/auth/create-api-key\n- https://bavlio.com/docs/api-reference/auth/revoke-api-key\n- https://bavlio.com/docs/authentication\ndescription: Authentication schemes for Bavlio API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Bearer authentication header of the form Bearer <token> , where <token> is your auth token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key via POST /api-keys (or receive a sign‑in token after registration) and use the returned secret as the Bearer\n    token.\nnote: No OAuth2, apiKey, or other authentication methods are documented.\ndocs: https://bavlio.com/docs/api-reference/auth/list-api-keys\n"
source_yaml_url: https://artifacts.apis.io/bavlio-com/authentication/bavlio-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Sales
- Outreach
- Automation
- Lead Generation
- Company
---
