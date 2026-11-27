---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tiquo-openapi-generated.yml
  format: yaml
  label: Tiquo Hospitality API
  slug: tiquo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tiquo/openapi/_ae-authored/tiquo-openapi-generated.yml
auth_types: []
description: Authentication methods for Tiquo APIs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Tiquo Hospitality Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tiquo Hospitality declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Tiquo Hospitality
provider_slug: tiquo
scheme_count: 1
schemes:
- evidence: The Admin API authenticates requests using API keys. These are organization‑scoped keys that you generate from the Tiquo dashboard. Include the key as a Bearer token in the Authorization header of every request.
  header: Authorization
  how_to_obtain: Generate an API key in the Tiquo dashboard under Settings > Admin API.
  location: header
  name: Admin API API Key
  type: http-bearer
slug: tiquo-authentication
source_filename: tiquo-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.tiquo.co/en/docs/api-reference/authentication
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.tiquo.co/en/docs/api-reference/authentication\nsources:\n- https://docs.tiquo.co/en/docs/api-reference/authentication\n- https://docs.tiquo.co/en/docs/api-reference/customer-api/token-refresh\n- https://docs.tiquo.co/en/docs/help/getting-started\n- https://docs.tiquo.co/en/docs/getting-started/account-setup\ndescription: Authentication methods for Tiquo APIs\nschemes:\n- type: http-bearer\n  name: Admin API API Key\n  evidence: The Admin API authenticates requests using API keys. These are organization‑scoped keys that you generate from the Tiquo dashboard.\n    Include the key as a Bearer token in the Authorization header of every request.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the Tiquo dashboard under Settings > Admin API.\nnote: No OAuth2 flow details (token or authorize URLs, scopes) are provided on the referenced\
  \ pages. 1 extracted row(s) were dropped because their\n  quote was not on the page.\ndocs: https://docs.tiquo.co/en/docs/api-reference/authentication\n"
source_yaml_url: https://artifacts.apis.io/tiquo/authentication/tiquo-authentication.yml
summary_line: 1 scheme
tags:
- Point-of-Sale
- Booking
- Payments
- Membership
- Marketing
- Hospitality Software
- Multi‑location Management
- Analytics
---
