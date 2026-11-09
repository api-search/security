---
anonymous_access: false
api_key_in: []
api_specs:
- filename: boundaryai-ai-openapi-generated.yml
  format: yaml
  label: BoundaryAI API
  slug: boundaryai-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boundaryai-ai/openapi/_ae-authored/boundaryai-ai-openapi-generated.yml
auth_types: []
description: BoundaryAI Python SDK authenticates using an API key passed to the SDK constructor or via the BOUNDARYAI_API_KEY environment variable.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Boundaryai Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: BoundaryAI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BoundaryAI
provider_slug: boundaryai-ai
scheme_count: 1
schemes:
- evidence: 'boundary = Boundary(api_key="bnd_live_...") # or BOUNDARYAI_API_KEY env var'
  name: api_key
  type: apiKey
slug: boundaryai-ai-authentication
source_filename: boundaryai-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://boundaryai.ai/docs/python-sdk
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://boundaryai.ai/docs/python-sdk\nsources:\n- https://boundaryai.ai/docs/python-sdk\ndescription: BoundaryAI Python SDK authenticates using an API key passed to the SDK constructor or via the BOUNDARYAI_API_KEY environment variable.\nschemes:\n- type: apiKey\n  name: api_key\n  evidence: 'boundary = Boundary(api_key=\"bnd_live_...\") # or BOUNDARYAI_API_KEY env var'\ndocs: https://boundaryai.ai/docs/python-sdk\n"
source_yaml_url: https://artifacts.apis.io/boundaryai-ai/authentication/boundaryai-ai-authentication.yml
summary_line: 1 scheme
tags:
- AI Governance
- Action enforcement
- Policy compliance
- Security
- Developer Tools
---
