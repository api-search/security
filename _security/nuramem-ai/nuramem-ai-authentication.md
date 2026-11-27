---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nuramem-ai-openapi-generated.yml
  format: yaml
  label: Nuramem API
  slug: nuramem-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuramem-ai/openapi/_ae-authored/nuramem-ai-openapi-generated.yml
auth_types: []
description: Authentication uses a bearer token passed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nuramem Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nuramem declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Nuramem
provider_slug: nuramem-ai
scheme_count: 1
schemes:
- evidence: 'The reference is OpenAPI, at https://nuramem.ai/openapi.json — fetch it with your token in the Authorization: Bearer header.'
  header: Authorization
  how_to_obtain: Sign in to the web app and get your token under Account → Data → API access.
  location: header
  name: Bearer token
  type: http-bearer
slug: nuramem-ai-authentication
source_filename: nuramem-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://nuramem.ai/docs/api/
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nuramem.ai/docs/api/\nsources:\n- https://nuramem.ai/docs/api/\ndescription: Authentication uses a bearer token passed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'The reference is OpenAPI, at https://nuramem.ai/openapi.json — fetch it with your token in the Authorization: Bearer header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in to the web app and get your token under Account → Data → API access.\ndocs: https://nuramem.ai/docs/api/\n"
source_yaml_url: https://artifacts.apis.io/nuramem-ai/authentication/nuramem-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Memory
- Collaboration
- Productivity
- Automation
---
