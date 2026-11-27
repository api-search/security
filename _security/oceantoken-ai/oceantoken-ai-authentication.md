---
anonymous_access: false
api_key_in: []
api_specs:
- filename: oceantoken-ai-openapi-generated.yml
  format: yaml
  label: OceanToken AI API
  slug: oceantoken-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oceantoken-ai/openapi/_ae-authored/oceantoken-ai-openapi-generated.yml
auth_types: []
description: Authentication schemes for OceanToken AI
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: OceanToken AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: OceanToken AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OceanToken AI
provider_slug: oceantoken-ai
scheme_count: 1
schemes:
- evidence: 'Send the key as a bearer token on every request: Authorization: Bearer sk-...'
  header: Authorization
  how_to_obtain: Create an API key in the OceanToken console and copy the key shown once.
  location: header
  name: API Key
  type: http-bearer
slug: oceantoken-ai-authentication
source_filename: oceantoken-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.oceantoken.ai/get-started/create-api-key
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.oceantoken.ai/get-started/create-api-key\nsources:\n- https://docs.oceantoken.ai/get-started/create-api-key\n- https://docs.oceantoken.ai/console/api-keys\n- https://docs.oceantoken.ai/zh-Hans/console/api-keys\n- https://docs.oceantoken.ai/zh-Hant/console/api-keys\ndescription: Authentication schemes for OceanToken AI\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Send the key as a bearer token on every request: Authorization: Bearer sk-...'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the OceanToken console and copy the key shown once.\nnote: No OAuth2 or other authentication methods are documented on the provided pages.\ndocs: https://docs.oceantoken.ai/get-started/create-api-key\n"
source_yaml_url: https://artifacts.apis.io/oceantoken-ai/authentication/oceantoken-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- LLM
- Text Generation
- Image Generation
- Video Generation
---
