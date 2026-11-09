---
anonymous_access: false
api_key_in: []
api_specs:
- filename: duvera-ai-openapi-generated.yml
  format: yaml
  label: Duvera API
  slug: duvera-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duvera-ai/openapi/_ae-authored/duvera-ai-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Duvera Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Duvera declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Duvera
provider_slug: duvera-ai
scheme_count: 1
schemes:
- evidence: your agent passes its own token at call time via the X-Duvera-Service-Token header — Duvera forwards it for that one call and never stores it
  header: X-Duvera-Service-Token
  location: header
  name: X-Duvera-Service-Token
  type: apiKey
slug: duvera-ai-authentication
source_filename: duvera-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://duvera.ai/quickstart
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://duvera.ai/quickstart\nsources:\n- https://duvera.ai/quickstart\ndescription: Authentication\nschemes:\n- type: apiKey\n  name: X-Duvera-Service-Token\n  evidence: your agent passes its own token at call time via the X-Duvera-Service-Token header — Duvera forwards it for that one call and never\n    stores it\n  location: header\n  header: X-Duvera-Service-Token\nnote: No OAuth2 or other authentication schemes are documented on the page.\ndocs: https://duvera.ai/quickstart\n"
source_yaml_url: https://artifacts.apis.io/duvera-ai/authentication/duvera-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI Governance
- Audit
- Compliance
- Enterprise
- Personal
---
