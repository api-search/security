---
anonymous_access: false
api_key_in: []
api_specs:
- filename: llmref-org-openapi-generated.yml
  format: yaml
  label: LLM Reference API
  slug: llmref-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmref-org/openapi/_ae-authored/llmref-org-openapi-generated.yml
auth_types: []
description: Authentication is optional. Anonymous requests are allowed; a valid API key only raises rate limits - it does not unlock data.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LLM Reference Authentication
name_suffix: Authentication
oauth_flows: []
overview: LLM Reference declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LLM Reference
provider_slug: llmref-org
scheme_count: 2
schemes:
- evidence: 'Send the key as a standard bearer token:'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
- evidence: The server also accepts the key in an x-api-key header as an alias.
  header: x-api-key
  location: header
  name: x-api-key
  type: apiKey
slug: llmref-org-authentication
source_filename: llmref-org-authentication.yml
source_heading: Authentication Profile
source_url: https://llmref.org/reference/rate-limits/
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://llmref.org/reference/rate-limits/\nsources:\n- https://llmref.org/reference/rate-limits/\ndescription: Authentication is optional. Anonymous requests are allowed; a valid API key only raises rate limits - it does not unlock data.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send the key as a standard bearer token:'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: x-api-key\n  evidence: The server also accepts the key in an x-api-key header as an alias.\n  location: header\n  header: x-api-key\nnote: 'If both are present, Authorization: Bearer wins.'\ndocs: https://llmref.org/reference/rate-limits/\n"
source_yaml_url: https://artifacts.apis.io/llmref-org/authentication/llmref-org-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Documentation
- Open Source
- Search
- Versioning
---
