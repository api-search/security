---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hellobooks-ai-openapi-generated.yml
  format: yaml
  label: HelloBooks AI API
  slug: hellobooks-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hellobooks-ai/openapi/_ae-authored/hellobooks-ai-openapi-generated.yml
auth_types: []
description: Authentication schemes for HelloBooks AI Public API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: HelloBooks AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: HelloBooks AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: HelloBooks AI
provider_slug: hellobooks-ai
scheme_count: 1
schemes:
- evidence: All /public/v1/* requests require a Bearer access token minted for a marketplace app install.
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: hellobooks-ai-authentication
source_filename: hellobooks-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://hellobooks.ai/docs/api-reference/foundations/authentication
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hellobooks.ai/docs/api-reference/foundations/authentication\nsources:\n- https://hellobooks.ai/docs/api-reference/foundations/authentication\n- https://hellobooks.ai/docs/api-reference/foundations\n- https://hellobooks.ai/docs/api-reference/foundations/tenant-isolation\n- https://hellobooks.ai/docs/api-reference/quickstarts/marketplace-app-setup\ndescription: Authentication schemes for HelloBooks AI Public API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: All /public/v1/* requests require a Bearer access token minted for a marketplace app install.\n  location: header\n  header: Authorization\ndocs: https://hellobooks.ai/docs/api-reference/foundations/authentication\n"
source_yaml_url: https://artifacts.apis.io/hellobooks-ai/authentication/hellobooks-ai-authentication.yml
summary_line: 1 scheme
tags:
- Accounting
- Artificial Intelligence
- Bookkeeping
- Small Business
- Software-as-a-Service
- Company
---
