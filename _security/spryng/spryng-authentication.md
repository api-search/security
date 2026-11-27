---
anonymous_access: false
api_key_in: []
api_specs:
- filename: spryng-openapi-generated.yml
  format: yaml
  label: Spryng API
  slug: spryng-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spryng/openapi/_ae-authored/spryng-openapi-generated.yml
auth_types: []
description: Authentication is performed via two required headers.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Spryng Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spryng declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Spryng
provider_slug: spryng
scheme_count: 2
schemes:
- evidence: These act like credentials on an envelope. This information must be provided in the Header of your request.
  header: X-API-Key
  location: header
  name: X-API-Key
  type: apiKey
- evidence: These act like credentials on an envelope. This information must be provided in the Header of your request.
  header: AccountReference
  location: header
  name: AccountReference
  type: apiKey
slug: spryng-authentication
source_filename: spryng-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.spryng.nl/two-factor-authentication/v2-otps-request
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.spryng.nl/two-factor-authentication/v2-otps-request\nsources:\n- https://developer.spryng.nl/two-factor-authentication/v2-otps-request\ndescription: Authentication is performed via two required headers.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: These act like credentials on an envelope. This information must be provided in the Header of your request.\n  location: header\n  header: X-API-Key\n- type: apiKey\n  name: AccountReference\n  evidence: These act like credentials on an envelope. This information must be provided in the Header of your request.\n  location: header\n  header: AccountReference\nnote: No OAuth2 or other authentication schemes are documented on the page.\ndocs: https://developer.spryng.nl/two-factor-authentication/v2-otps-request\n"
source_yaml_url: https://artifacts.apis.io/spryng/authentication/spryng-authentication.yml
summary_line: 2 schemes
tags:
- Messaging
- SMS
- RCS
- WhatsApp Business
- Voice API
---
