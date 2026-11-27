---
anonymous_access: false
api_key_in: []
api_specs:
- filename: edgaze-ai-runs-api-openapi.yml
  format: yaml
  label: Edgaze Runs API
  slug: edgaze-ai-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgaze-ai/openapi/edgaze-ai-runs-api-openapi.yml
- filename: edgaze-ai-workflows-api-openapi.yml
  format: yaml
  label: Edgaze Workflows API
  slug: edgaze-ai-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgaze-ai/openapi/edgaze-ai-workflows-api-openapi.yml
auth_types: []
description: Every API request must include a valid secret key in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Edgaze Authentication
name_suffix: Authentication
oauth_flows: []
overview: Edgaze declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Edgaze
provider_slug: edgaze-ai
scheme_count: 1
schemes:
- evidence: Every API request must include a valid secret key in the Authorization header.
  header: Authorization
  how_to_obtain: Create and manage keys in the Developer console.
  location: header
  name: Bearer
  type: http-bearer
slug: edgaze-ai-authentication
source_filename: edgaze-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.edgaze.ai/docs/api/authentication.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.edgaze.ai/docs/api/authentication.md\nsources:\n- https://www.edgaze.ai/docs/api/authentication.md\n- https://www.edgaze.ai/docs/api/authentication\n- https://www.edgaze.ai/docs/billing/byok\n- https://www.edgaze.ai/developer/keys\ndescription: Every API request must include a valid secret key in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Every API request must include a valid secret key in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create and manage keys in the Developer console.\ndocs: https://www.edgaze.ai/docs/api/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/edgaze-ai/authentication/edgaze-ai-authentication.yml
summary_line: 1 scheme
tags:
- Marketplace
- AI Workflows
- Creator Program
- Per‑run Pricing
- Workflow Studio
---
