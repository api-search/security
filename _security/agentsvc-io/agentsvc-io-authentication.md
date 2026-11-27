---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses an API key sent as a bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agentsvc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agentsvc declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Agentsvc
provider_slug: agentsvc-io
scheme_count: 1
schemes:
- evidence: Prepay once, then your agent calls any service with a bearer token.
  header: Authorization
  how_to_obtain: Get an API key from the credits page (https://agentsvc.io/credits) and use it as a Bearer token.
  location: header
  name: API Key
  type: http-bearer
slug: agentsvc-io-authentication
source_filename: agentsvc-io-authentication.yml
source_heading: Authentication Profile
source_url: https://agentsvc.io/credits
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agentsvc.io/credits\nsources:\n- https://agentsvc.io/credits\n- https://agentsvc.io/guides/check-token-before-swap\n- https://agentsvc.io/services/token-security\n- https://agentsvc.io/services/token-verdict\ndescription: Authentication uses an API key sent as a bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Prepay once, then your agent calls any service with a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Get an API key from the credits page (https://agentsvc.io/credits) and use it as a Bearer token.\ndocs: https://agentsvc.io/credits\n"
source_yaml_url: https://artifacts.apis.io/agentsvc-io/authentication/agentsvc-io-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Marketplace
- Payments
- Web Services
- Agents
---
