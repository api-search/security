---
anonymous_access: false
api_key_in: []
api_specs:
- filename: syntology-ai-openapi-generated.yml
  format: yaml
  label: Syntology API
  slug: syntology-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/syntology-ai/openapi/_ae-authored/syntology-ai-openapi-generated.yml
auth_types: []
description: Authentication schemes as published on the Syntology documentation pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Syntology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Syntology declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Syntology
provider_slug: syntology-ai
scheme_count: 1
schemes:
- evidence: 'Trial token without a full OAuth UI curl -X POST https://syntology.ai/api/oauth/trial/token \ -H "Content-Type: application/json" \ -d ''{"grant_type":"client_credentials"}'''
  flows:
  - client_credentials
  how_to_obtain: Obtain a token by sending a POST request to the token URL with grant_type=client_credentials.
  name: OAuth2 Trial
  token_url: https://syntology.ai/api/oauth/trial/token
  type: oauth2
slug: syntology-ai-authentication
source_filename: syntology-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://app.syntology.ai/docs/how-to/atlas-quickstart/
source_yaml: "generated: '2026-11-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://app.syntology.ai/docs/how-to/atlas-quickstart/\nsources:\n- https://app.syntology.ai/docs/how-to/atlas-quickstart/\n- https://app.syntology.ai/docs/agents/mcp/\ndescription: Authentication schemes as published on the Syntology documentation pages.\nschemes:\n- type: oauth2\n  name: OAuth2 Trial\n  evidence: 'Trial token without a full OAuth UI curl -X POST https://syntology.ai/api/oauth/trial/token \\ -H \"Content-Type: application/json\"\n    \\ -d ''{\"grant_type\":\"client_credentials\"}'''\n  flows:\n  - client_credentials\n  token_url: https://syntology.ai/api/oauth/trial/token\n  how_to_obtain: Obtain a token by sending a POST request to the token URL with grant_type=client_credentials.\ndocs: https://app.syntology.ai/docs/how-to/atlas-quickstart/\n"
source_yaml_url: https://artifacts.apis.io/syntology-ai/authentication/syntology-ai-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Ontology
- GraphAPI
- OpenData
- Research
---
