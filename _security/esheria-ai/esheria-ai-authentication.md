---
anonymous_access: false
api_key_in: []
api_specs:
- filename: esheria-ai-openapi-generated.yml
  format: yaml
  label: Esheria API
  slug: esheria-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esheria-ai/openapi/_ae-authored/esheria-ai-openapi-generated.yml
auth_types: []
description: Authentication schemes for Esheria API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Esheria Authentication
name_suffix: Authentication
oauth_flows: []
overview: Esheria declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Esheria
provider_slug: esheria-ai
scheme_count: 1
schemes:
- evidence: Protected endpoints require an API key in the `x-api-key` header.
  header: x-api-key
  how_to_obtain: Create self-serve API tokens from https://dashboard.esheria.ai/.
  location: header
  name: API Key
  type: apiKey
slug: esheria-ai-authentication
source_filename: esheria-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.esheria.ai/guides/authentication.md
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.esheria.ai/guides/authentication.md\nsources:\n- https://docs.esheria.ai/guides/authentication.md\n- https://docs.esheria.ai/guides/api-keys.md\n- https://docs.esheria.ai/api-reference/oauth-protected-resource-metadata.md\n- https://docs.esheria.ai/api-reference/oauth-authorization-server-metadata.md\ndescription: Authentication schemes for Esheria API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Protected endpoints require an API key in the `x-api-key` header.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create self-serve API tokens from https://dashboard.esheria.ai/.\nnote: No OAuth2 or other authentication schemes are documented on the provided pages.\ndocs: https://docs.esheria.ai/guides/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/esheria-ai/authentication/esheria-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Legal AI
- Regulatory Intelligence
- Africa
- Compliance
---
