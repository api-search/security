---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cosmic-ephemeris-calculations-api-openapi.yml
  format: yaml
  label: Cosmic Ephemeris Calculations API
  slug: cosmic-ephemeris-calculations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmic-ephemeris/openapi/cosmic-ephemeris-calculations-api-openapi.yml
- filename: cosmic-ephemeris-interpretation-api-openapi.yml
  format: yaml
  label: Cosmic Ephemeris Interpretation API
  slug: cosmic-ephemeris-interpretation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmic-ephemeris/openapi/cosmic-ephemeris-interpretation-api-openapi.yml
- filename: cosmic-ephemeris-pro-timeline-api-openapi.yml
  format: yaml
  label: Cosmic Ephemeris Pro timeline API
  slug: cosmic-ephemeris-pro-timeline-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmic-ephemeris/openapi/cosmic-ephemeris-pro-timeline-api-openapi.yml
auth_types: []
description: Authentication methods for Cosmic Ephemeris API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cosmic Ephemeris Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cosmic Ephemeris declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cosmic Ephemeris
provider_slug: cosmic-ephemeris
scheme_count: 2
schemes:
- evidence: 'Send it using the preferred Bearer header: Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Generated in the dashboard; full plaintext shown only when a key is generated or regenerated.
  name: Bearer
  type: http-bearer
- evidence: 'The equivalent header below is also supported: x-api-key: YOUR_API_KEY'
  header: x-api-key
  how_to_obtain: Generated in the dashboard; full plaintext shown only when a key is generated or regenerated.
  location: header
  name: x-api-key
  type: apiKey
slug: cosmic-ephemeris-authentication
source_filename: cosmic-ephemeris-authentication.yml
source_heading: Authentication Profile
source_url: https://cosmicephemeris.com/docs-auth.html
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cosmicephemeris.com/docs-auth.html\nsources:\n- https://cosmicephemeris.com/docs-auth.html\n- https://cosmicephemeris.com/docs-onboarding-context.html\ndescription: Authentication methods for Cosmic Ephemeris API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send it using the preferred Bearer header: Authorization: Bearer YOUR_API_KEY'\n  header: Authorization\n  how_to_obtain: Generated in the dashboard; full plaintext shown only when a key is generated or regenerated.\n- type: apiKey\n  name: x-api-key\n  evidence: 'The equivalent header below is also supported: x-api-key: YOUR_API_KEY'\n  location: header\n  header: x-api-key\n  how_to_obtain: Generated in the dashboard; full plaintext shown only when a key is generated or regenerated.\nnote: No OAuth2 flows are documented.\ndocs: https://cosmicephemeris.com/docs-auth.html\n"
source_yaml_url: https://artifacts.apis.io/cosmic-ephemeris/authentication/cosmic-ephemeris-authentication.yml
summary_line: 2 schemes
tags:
- Astrology
- API
- Developer
- Data
- U.S.-based
---
