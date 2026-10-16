---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cnaught-openapi-generated.yml
  format: yaml
  label: CNaught API
  slug: cnaught-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cnaught/refs/heads/main/openapi/_ae-authored/cnaught-openapi-generated.yml
auth_types: []
description: Authentication uses an API key provided as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cnaught Authentication
name_suffix: Authentication
oauth_flows: []
overview: CNaught declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CNaught
provider_slug: cnaught
scheme_count: 1
schemes:
- evidence: Replace the `<CNAUGHT_API_KEY>` placeholder with the API key obtained in Step 1, and specify the amount of carbon credits (in kg of CO2e) you wish to purchase.
  header: Authorization
  how_to_obtain: Generate an API key via the Developers page after logging in to CNaught.
  location: header
  name: Bearer
  type: http-bearer
slug: cnaught-authentication
source_filename: cnaught-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.cnaught.com/quickstart.md
source_yaml: "generated: '2026-10-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.cnaught.com/quickstart.md\nsources:\n- https://docs.cnaught.com/quickstart.md\ndescription: Authentication uses an API key provided as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Replace the `<CNAUGHT_API_KEY>` placeholder with the API key obtained in Step 1, and specify the amount of carbon credits (in kg of\n    CO2e) you wish to purchase.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key via the Developers page after logging in to CNaught.\ndocs: https://docs.cnaught.com/quickstart.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cnaught/refs/heads/main/authentication/cnaught-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Climate
- CarbonCredits
- API
- Sustainability
---
