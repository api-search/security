---
anonymous_access: false
api_key_in: []
api_specs:
- filename: infere-openapi-generated.yml
  format: yaml
  label: Snowball Studio Ltd. API
  slug: infere-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infere/refs/heads/main/openapi/_ae-authored/infere-openapi-generated.yml
auth_types: []
description: Authentication schemes for Infere
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Infere Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snowball Studio Ltd. declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Snowball Studio Ltd.
provider_slug: infere
scheme_count: 1
schemes:
- evidence: API tokens are the primary authentication mechanism for the Infere platform.
  header: Authorization
  location: header
  name: API token
  type: http-bearer
slug: infere-authentication
source_filename: infere-authentication.yml
source_heading: Authentication Profile
source_url: https://infere.com/documentation/token-management/
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://infere.com/documentation/token-management/\nsources:\n- https://infere.com/documentation/token-management/\n- https://infere.com/glossary/api-token/\n- https://infere.com/glossary/token/\n- https://infere.com/glossary/token-budget/\ndescription: Authentication schemes for Infere\nschemes:\n- type: http-bearer\n  name: API token\n  evidence: API tokens are the primary authentication mechanism for the Infere platform.\n  location: header\n  header: Authorization\ndocs: https://infere.com/documentation/token-management/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infere/refs/heads/main/authentication/infere-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Observability
- PromptManagement
- LLM
---
