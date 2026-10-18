---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Jedlix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jedlix declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Jedlix
provider_slug: jedlix
scheme_count: 1
schemes:
- evidence: During the setup process, you will be provided with an API key, and you should include this in every interaction with the Smart Charging API.
  header: ApiKey
  how_to_obtain: Contact the sales team (mailto:partners@jedlix.com) to receive an API key during the setup process.
  location: header
  name: ApiKey
  type: apiKey
slug: jedlix-authentication
source_filename: jedlix-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.jedlix.com/docs/authorization.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.jedlix.com/docs/authorization.md\nsources:\n- https://developer.jedlix.com/docs/authorization.md\n- https://developer.jedlix.com/docs/api-key.md\n- https://developer.jedlix.com/reference/submitconnectsessioninfo.md\n- https://developer.jedlix.com/docs/management-access-token.md\nschemes:\n- type: apiKey\n  name: ApiKey\n  evidence: During the setup process, you will be provided with an API key, and you should include this in every interaction with the Smart Charging\n    API.\n  location: header\n  header: ApiKey\n  how_to_obtain: Contact the sales team (mailto:partners@jedlix.com) to receive an API key during the setup process.\ndocs: https://developer.jedlix.com/docs/authorization.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jedlix/refs/heads/main/authentication/jedlix-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Fintech
- Electric Vehicles
- Charging
- Energy
---
