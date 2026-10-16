---
anonymous_access: false
api_key_in: []
api_specs:
- filename: plugsurfing-reference-openapi.json
  format: json
  label: Drive API Reference API
  slug: drive-api-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/openapi/_original/plugsurfing-reference-openapi.json
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Plugsurfing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plugsurfing declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Plugsurfing
provider_slug: plugsurfing
scheme_count: 1
schemes:
- evidence: Every API request must include the API key in the `X-API-Key` header.
  header: X-API-Key
  how_to_obtain: You can obtain the API key from the Control Panel for both stage and production environments (ask your CSM for access).
  location: header
  name: X-API-Key
  type: apiKey
slug: plugsurfing-authentication
source_filename: plugsurfing-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.plugsurfing.com/docs/drive-api/authorization.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.plugsurfing.com/docs/drive-api/authorization.md\nsources:\n- https://developer.plugsurfing.com/docs/drive-api/authorization.md\n- https://developer.plugsurfing.com/reference/getStripePublishableApiKey.md\n- https://developer.plugsurfing.com/docs/drive-api/authorization\n- https://developer.plugsurfing.com/docs/roam-ocpi/credentials-module.md\ndescription: Authentication\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Every API request must include the API key in the `X-API-Key` header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: You can obtain the API key from the Control Panel for both stage and production environments (ask your CSM for access).\ndocs: https://developer.plugsurfing.com/docs/drive-api/authorization.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plugsurfing/refs/heads/main/authentication/plugsurfing-authentication.yml
summary_line: 1 scheme
tags:
- Company
- EVCharging
- API
- Roaming
- Europe
---
