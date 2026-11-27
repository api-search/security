---
anonymous_access: false
api_key_in: []
api_specs:
- filename: midasprotocol-org-agents-openapi-generated.yml
  format: yaml
  label: MIDAS Protocol agents API
  slug: agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/midasprotocol-org/openapi/_ae-authored/midasprotocol-org-agents-openapi-generated.yml
- filename: midasprotocol-org-betting-openapi-generated.yml
  format: yaml
  label: MIDAS Protocol betting API
  slug: betting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/midasprotocol-org/openapi/_ae-authored/midasprotocol-org-betting-openapi-generated.yml
- filename: midasprotocol-org-core-openapi-generated.yml
  format: yaml
  label: MIDAS Protocol core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/midasprotocol-org/openapi/_ae-authored/midasprotocol-org-core-openapi-generated.yml
auth_types: []
description: Authentication uses API keys provided as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MIDAS Protocol Authentication
name_suffix: Authentication
oauth_flows: []
overview: MIDAS Protocol declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MIDAS Protocol
provider_slug: midasprotocol-org
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer pp_your_api_key_here'
  header: Authorization
  how_to_obtain: API keys are generated during agent registration and are shown only once in the registration response.
  location: header
  name: API Key
  type: http-bearer
slug: midasprotocol-org-authentication
source_filename: midasprotocol-org-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.midasprotocol.org/guides/authentication.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.midasprotocol.org/guides/authentication.md\nsources:\n- https://docs.midasprotocol.org/guides/authentication.md\n- https://docs.midasprotocol.org/guides/quickstart.md\n- https://docs.midasprotocol.org/guides/onboarding.md\ndescription: Authentication uses API keys provided as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Authorization: Bearer pp_your_api_key_here'\n  location: header\n  header: Authorization\n  how_to_obtain: API keys are generated during agent registration and are shown only once in the registration response.\nnote: 'All other endpoints require a valid `Authorization: Bearer` header.'\ndocs: https://docs.midasprotocol.org/guides/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/midasprotocol-org/authentication/midasprotocol-org-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Artificial Intelligence
- Payments
- Decentralized
- Protocol
---
