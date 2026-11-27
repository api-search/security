---
anonymous_access: false
api_key_in: []
api_specs:
- filename: multinex-ai-openapi-generated.yml
  format: yaml
  label: Multinex AI API
  slug: multinex-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multinex-ai/openapi/_ae-authored/multinex-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for MemQ as documented.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Multinex AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Multinex AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Multinex AI
provider_slug: multinex-ai
scheme_count: 1
schemes:
- evidence: '"Authorization": "Bearer ${MEMQ_API_KEY}"'
  header: Authorization
  location: header
  name: MEMQ_API_KEY
  type: http-bearer
slug: multinex-ai-authentication
source_filename: multinex-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://multinex.ai/docs/memq/quickstart/
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://multinex.ai/docs/memq/quickstart/\nsources:\n- https://multinex.ai/docs/memq/quickstart/\n- https://multinex.ai/docs/memq/editors/\ndescription: Authentication methods for MemQ as documented.\nschemes:\n- type: http-bearer\n  name: MEMQ_API_KEY\n  evidence: '\"Authorization\": \"Bearer ${MEMQ_API_KEY}\"'\n  location: header\n  header: Authorization\nnote: OAuth sign‑in is mentioned but no token or authorize URLs, flows, or scopes are provided on the pages.\ndocs: https://multinex.ai/docs/memq/quickstart/\n"
source_yaml_url: https://artifacts.apis.io/multinex-ai/authentication/multinex-ai-authentication.yml
summary_line: 1 scheme
tags:
- AI Memory
- Enterprise AI
- Data Protection
---
