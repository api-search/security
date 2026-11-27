---
anonymous_access: false
api_key_in: []
api_specs:
- filename: funkel-ai-openapi-generated.yml
  format: yaml
  label: Funkel AI API
  slug: funkel-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/funkel-ai/openapi/_ae-authored/funkel-ai-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Funkel AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Funkel AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Funkel AI
provider_slug: funkel-ai
scheme_count: 1
schemes:
- evidence: Send the token in the Authorization header.
  header: Authorization
  how_to_obtain: Create a token in Settings → Security in the Funkel AI app; the token value begins with funkel_pat_ and must be copied immediately.
  location: header
  name: Personal Access Token
  type: http-bearer
slug: funkel-ai-authentication
source_filename: funkel-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://funkel.ai/doc/authentication
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://funkel.ai/doc/authentication\nsources:\n- https://funkel.ai/doc/authentication\n- https://funkel.ai/doc/getting-started\n- https://funkel.ai/help/getting-started/create-your-workspace\n- https://funkel.ai/help/getting-started/launch-your-first-campaign\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Personal Access Token\n  evidence: Send the token in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token in Settings → Security in the Funkel AI app; the token value begins with funkel_pat_ and must be copied immediately.\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the provided pages.\ndocs: https://funkel.ai/doc/authentication\n"
source_yaml_url: https://artifacts.apis.io/funkel-ai/authentication/funkel-ai-authentication.yml
summary_line: 1 scheme
tags:
- B2B
- Sales Automation
- Lead Generation
- Artificial Intelligence
- Marketing
---
