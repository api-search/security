---
anonymous_access: false
api_key_in: []
api_specs:
- filename: enginy-ai-openapi-generated.yml
  format: yaml
  label: Enginy API
  slug: enginy-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enginy-ai/openapi/_ae-authored/enginy-ai-openapi-generated.yml
auth_types: []
description: Enginy supports API key authentication via a header. The API key can be sent either as the `x-api-key` header or as a Bearer token in the `Authorization` header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Enginy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enginy declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Enginy
provider_slug: enginy-ai
scheme_count: 1
schemes:
- evidence: "components:\n  securitySchemes:\n    apiKey:\n      type: apiKey\n      in: header\n      name: x-api-key"
  header: x-api-key
  location: header
  name: apiKey
  type: apiKey
slug: enginy-ai-authentication
source_filename: enginy-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.enginy.ai/api-reference/authentication/validate-api-key.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.enginy.ai/api-reference/authentication/validate-api-key.md\nsources:\n- https://docs.enginy.ai/api-reference/authentication/validate-api-key.md\n- https://docs.enginy.ai/mcp/api-key-auth.md\n- https://help.enginy.ai/en/collections/9565147-start-here\ndescription: Enginy supports API key authentication via a header. The API key can be sent either as the `x-api-key` header or as a Bearer token\n  in the `Authorization` header.\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: \"components:\\n  securitySchemes:\\n    apiKey:\\n      type: apiKey\\n      in: header\\n      name: x-api-key\"\n  location: header\n  header: x-api-key\ndocs: https://docs.enginy.ai/api-reference/authentication/validate-api-key.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/enginy-ai/authentication/enginy-ai-authentication.yml
summary_line: 1 scheme
tags:
- B2B
- Sales
- Artificial Intelligence
- Lead Enrichment
- Marketing
---
