---
anonymous_access: false
api_key_in: []
api_specs:
- filename: esimoa-com-countries-api-openapi.yml
  format: yaml
  label: esimoa Countries API
  slug: esimoa-com-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimoa-com/openapi/esimoa-com-countries-api-openapi.yml
- filename: esimoa-com-esims-api-openapi.yml
  format: yaml
  label: esimoa Esims API
  slug: esimoa-com-esims-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimoa-com/openapi/esimoa-com-esims-api-openapi.yml
auth_types: []
description: Authentication schemes for esimoa APIs
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: esimoa Authentication
name_suffix: Authentication
oauth_flows: []
overview: esimoa declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: esimoa
provider_slug: esimoa-com
scheme_count: 4
schemes:
- evidence: Send your API key in a header with every request. Keys start with esk_live_; use whichever header is convenient.
  header: X-API-Key
  how_to_obtain: Create a key in the Developer Center dashboard; the key is shown only once when created.
  location: header
  name: Public API key
  type: apiKey
- evidence: Send your API key in a header with every request. Keys start with esk_live_; use whichever header is convenient.
  header: Authorization
  how_to_obtain: Create a key in the Developer Center dashboard; the key is shown only once when created.
  location: header
  name: Public API Bearer token
  type: apiKey
- evidence: 'Send the key in the X-API-Key header on every request; Authorization: Bearer is also accepted.'
  header: X-API-Key
  how_to_obtain: Create a key in the partner portal; the full key is displayed only once at issue time.
  location: header
  name: Partner API key
  type: apiKey
- evidence: 'Send the key in the X-API-Key header on every request; Authorization: Bearer is also accepted.'
  header: Authorization
  how_to_obtain: Create a key in the partner portal; the full key is displayed only once at issue time.
  location: header
  name: Partner API Bearer token
  type: apiKey
slug: esimoa-com-authentication
source_filename: esimoa-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.esimoa.com/en/developers/docs/authentication
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.esimoa.com/en/developers/docs/authentication\nsources:\n- https://www.esimoa.com/en/developers/docs/authentication\n- https://www.esimoa.com/en/developers/docs/partner-api/authentication\n- https://esimoa.com/en/developers/docs/authentication\n- https://esimoa.com/en/developers/docs/partner-api/authentication\ndescription: Authentication schemes for esimoa APIs\nschemes:\n- type: apiKey\n  name: Public API key\n  evidence: Send your API key in a header with every request. Keys start with esk_live_; use whichever header is convenient.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a key in the Developer Center dashboard; the key is shown only once when created.\n- type: apiKey\n  name: Public API Bearer token\n  evidence: Send your API key in a header with every request. Keys start with esk_live_; use whichever header is convenient.\n  location: header\n\
  \  header: Authorization\n  how_to_obtain: Create a key in the Developer Center dashboard; the key is shown only once when created.\n- type: apiKey\n  name: Partner API key\n  evidence: 'Send the key in the X-API-Key header on every request; Authorization: Bearer is also accepted.'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a key in the partner portal; the full key is displayed only once at issue time.\n- type: apiKey\n  name: Partner API Bearer token\n  evidence: 'Send the key in the X-API-Key header on every request; Authorization: Bearer is also accepted.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the partner portal; the full key is displayed only once at issue time.\ndocs: https://www.esimoa.com/en/developers/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/esimoa-com/authentication/esimoa-com-authentication.yml
summary_line: 4 schemes
tags:
- eSIM
- Travel
- Price Comparison
- Mobile Data
- International
---
