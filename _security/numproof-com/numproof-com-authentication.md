---
anonymous_access: false
api_key_in: []
api_specs:
- filename: numproof-com-api-openapi.json
  format: json
  label: NumProof Api API
  slug: numproof-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/numproof-com/openapi/_original/numproof-com-api-openapi.json
auth_types: []
description: NumProof uses an API key provided as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: NumProof Authentication
name_suffix: Authentication
oauth_flows: []
overview: NumProof declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: NumProof
provider_slug: numproof-com
scheme_count: 1
schemes:
- evidence: 'Use your key First request curl -X POST https://numproof.com/verify \ -H "Authorization: Bearer vk_…" \ -H "Content-Type: application/json" \ -d ''{"claim":"(R-C)/R == 1 - C/R"}'''
  header: Authorization
  how_to_obtain: Mint a sandbox key Calls POST /signup. Store the key shown — it is displayed once.
  location: header
  name: Authorization
  type: http-bearer
slug: numproof-com-authentication
source_filename: numproof-com-authentication.yml
source_heading: Authentication Profile
source_url: https://numproof.com/start
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://numproof.com/start\nsources:\n- https://numproof.com/start\ndescription: NumProof uses an API key provided as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Use your key First request curl -X POST https://numproof.com/verify \\ -H \"Authorization: Bearer vk_…\" \\ -H \"Content-Type: application/json\"\n    \\ -d ''{\"claim\":\"(R-C)/R == 1 - C/R\"}'''\n  location: header\n  header: Authorization\n  how_to_obtain: Mint a sandbox key Calls POST /signup. Store the key shown — it is displayed once.\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the page.\ndocs: https://numproof.com/start\n"
source_yaml_url: https://artifacts.apis.io/numproof-com/authentication/numproof-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Finance
- Verification
- Zero Trust
---
