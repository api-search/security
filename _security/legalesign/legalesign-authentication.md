---
anonymous_access: false
api_key_in: []
auth_types: []
description: Legalesign authenticates API requests using a Developer Portal API key sent as a bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Legalesign Authentication
name_suffix: Authentication
oauth_flows: []
overview: Legalesign declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Legalesign
provider_slug: legalesign
scheme_count: 1
schemes:
- evidence: 'Send the Developer Portal key as a bearer token: Authorization: Bearer ak_<environment>_<key-id>.<secret>'
  header: Authorization
  how_to_obtain: Create an API key in the Legalesign Developer Portal and use the generated key in the Authorization header as shown.
  location: header
  name: Authorization
  type: http-bearer
slug: legalesign-authentication
source_filename: legalesign-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.legalesign.com/tags/api-key
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.legalesign.com/tags/api-key\nsources:\n- https://docs.legalesign.com/tags/api-key\n- https://docs.legalesign.com/tags/authentication\n- https://docs.legalesign.com/graphql/reference/api-key\n- https://docs.legalesign.com/graphql/reference/enums/recipient-authentication\ndescription: Legalesign authenticates API requests using a Developer Portal API key sent as a bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Send the Developer Portal key as a bearer token: Authorization: Bearer ak_<environment>_<key-id>.<secret>'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the Legalesign Developer Portal and use the generated key in the Authorization header as shown.\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the provided pages.\ndocs: https://docs.legalesign.com/tags/api-key\n"
source_yaml_url: https://artifacts.apis.io/legalesign/authentication/legalesign-authentication.yml
summary_line: 1 scheme
tags:
- Company
- E-Signature
- Automation
- Document Management
---
