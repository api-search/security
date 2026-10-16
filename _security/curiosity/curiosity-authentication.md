---
anonymous_access: false
api_key_in: []
api_specs:
- filename: curiosity-openapi-generated.yml
  format: yaml
  label: Curiosity API
  slug: curiosity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/_ae-authored/curiosity-openapi-generated.yml
auth_types: []
description: Curiosity uses bearer tokens passed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Curiosity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Curiosity declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Curiosity
provider_slug: curiosity
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer <endpoint-token>'
  header: Authorization
  how_to_obtain: Created via Admin → API Tokens (API token, Endpoint token) or via login flow for Session JWT.
  location: header
  name: API token / Endpoint token / Session JWT
  type: http-bearer
slug: curiosity-authentication
source_filename: curiosity-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.curiosity.ai/workspace-learning/07-apis-endpoints/02-authentication
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.curiosity.ai/workspace-learning/07-apis-endpoints/02-authentication\nsources:\n- https://docs.curiosity.ai/workspace-learning/07-apis-endpoints/02-authentication\n- https://docs.curiosity.ai/workspace/getting-started/build-your-first-enterprise-ai-app\ndescription: Curiosity uses bearer tokens passed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API token / Endpoint token / Session JWT\n  evidence: 'Authorization: Bearer <endpoint-token>'\n  location: header\n  header: Authorization\n  how_to_obtain: Created via Admin → API Tokens (API token, Endpoint token) or via login flow for Session JWT.\nnote: No OAuth2, apiKey, http-basic, jwt, hmac, mtls, or other schemes are documented on the referenced pages.\ndocs: https://docs.curiosity.ai/workspace-learning/07-apis-endpoints/02-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/authentication/curiosity-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Knowledge-Graph
- Enterprise
- Data-Integration
- On-Premises
- Company
---
