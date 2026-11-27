---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ismscopilot-com-docs-api-openapi.yml
  format: yaml
  label: ISMS Copilot Docs API
  slug: ismscopilot-com-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismscopilot-com/openapi/ismscopilot-com-docs-api-openapi.yml
- filename: ismscopilot-com-public-feeds-api-openapi.yml
  format: yaml
  label: ISMS Copilot Public Feeds API
  slug: ismscopilot-com-public-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ismscopilot-com/openapi/ismscopilot-com-public-feeds-api-openapi.yml
auth_types: []
description: Authentication schemes for ISMS Copilot API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ISMS Copilot Authentication
name_suffix: Authentication
oauth_flows: []
overview: ISMS Copilot declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ISMS Copilot
provider_slug: ismscopilot-com
scheme_count: 1
schemes:
- evidence: 'curl https://api.ismscopilot.com/v1/chat/completions \ -H "Authorization: Bearer sk-isms-..."'
  header: Authorization
  how_to_obtain: Create a key in the platform console; the key starts with sk-isms- and is shown only once.
  location: header
  name: Bearer
  type: http-bearer
slug: ismscopilot-com-authentication
source_filename: ismscopilot-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ismscopilot.com/docs/api/get-api-key
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ismscopilot.com/docs/api/get-api-key\nsources:\n- https://docs.ismscopilot.com/docs/api/get-api-key\n- https://docs.ismscopilot.com/docs/agents/token-and-cost\n- https://docs.ismscopilot.com/docs/agents/tokens-and-scopes\n- https://docs.ismscopilot.com/docs/agents/connect-cursor-and-codex\ndescription: Authentication schemes for ISMS Copilot API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl https://api.ismscopilot.com/v1/chat/completions \\ -H \"Authorization: Bearer sk-isms-...\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the platform console; the key starts with sk-isms- and is shown only once.\nnote: OAuth sign‑in is described but no token or authorize URLs, flows, or scopes are provided on the pages, so no OAuth scheme is listed.\ndocs: https://docs.ismscopilot.com/docs/api/get-api-key\n"
source_yaml_url: https://artifacts.apis.io/ismscopilot-com/authentication/ismscopilot-com-authentication.yml
summary_line: 1 scheme
tags:
- GRC
- Artificial Intelligence
- Compliance
- ISO 27001
- SOC 2
---
