---
anonymous_access: false
api_key_in: []
api_specs:
- filename: flightpowers-com-account-api-openapi.yml
  format: yaml
  label: flightpowers-com Account API
  slug: flightpowers-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightpowers-com/openapi/flightpowers-com-account-api-openapi.yml
- filename: flightpowers-com-flights-api-openapi.yml
  format: yaml
  label: flightpowers-com Flights API
  slug: flightpowers-com-flights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightpowers-com/openapi/flightpowers-com-flights-api-openapi.yml
- filename: flightpowers-com-hotels-api-openapi.yml
  format: yaml
  label: flightpowers-com Hotels API
  slug: flightpowers-com-hotels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightpowers-com/openapi/flightpowers-com-hotels-api-openapi.yml
- filename: flightpowers-com-verify-api-openapi.yml
  format: yaml
  label: flightpowers-com Verify API
  slug: flightpowers-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flightpowers-com/openapi/flightpowers-com-verify-api-openapi.yml
auth_types: []
description: Authentication uses a RapidAPI key that can be sent in a header or query string, or as a Bearer token.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Flightpowers Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: flightpowers-com declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: flightpowers-com
provider_slug: flightpowers-com
scheme_count: 3
schemes:
- evidence: 'The key goes in x-api-key , x-rapidapi-key , or Authorization: Bearer , whichever your client makes easiest.'
  header: x-rapidapi-key
  how_to_obtain: Obtain a RapidAPI key from RapidAPI (or use the free sign‑in key provided after Google sign‑in).
  location: header
  name: x-rapidapi-key
  type: apiKey
- evidence: 'Clients that take only a URL and no headers can put the key on the URL: key on the URL https://flights.flightpowers.com/mcp?rapidapi_key=YOUR_RAPIDAPI_KEY'
  how_to_obtain: Obtain a RapidAPI key from RapidAPI (or use the free sign‑in key provided after Google sign‑in).
  location: query
  name: rapidapi_key
  type: apiKey
- evidence: 'The key goes in x-api-key , x-rapidapi-key , or Authorization: Bearer , whichever your client makes easiest.'
  header: Authorization
  how_to_obtain: Obtain a RapidAPI key from RapidAPI (or use the free sign‑in key provided after Google sign‑in).
  location: header
  name: Authorization
  type: http-bearer
slug: flightpowers-com-authentication
source_filename: flightpowers-com-authentication.yml
source_heading: Authentication Profile
source_url: https://flightpowers.com/mcp
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://flightpowers.com/mcp\nsources:\n- https://flightpowers.com/mcp\n- https://flightpowers.com/docs/quickstart\ndescription: Authentication uses a RapidAPI key that can be sent in a header or query string, or as a Bearer token.\nschemes:\n- type: apiKey\n  name: x-rapidapi-key\n  evidence: 'The key goes in x-api-key , x-rapidapi-key , or Authorization: Bearer , whichever your client makes easiest.'\n  location: header\n  header: x-rapidapi-key\n  how_to_obtain: Obtain a RapidAPI key from RapidAPI (or use the free sign‑in key provided after Google sign‑in).\n- type: apiKey\n  name: rapidapi_key\n  evidence: 'Clients that take only a URL and no headers can put the key on the URL: key on the URL https://flights.flightpowers.com/mcp?rapidapi_key=YOUR_RAPIDAPI_KEY'\n  location: query\n  how_to_obtain: Obtain a RapidAPI key from RapidAPI (or use the free sign‑in key provided after\
  \ Google sign‑in).\n- type: http-bearer\n  name: Authorization\n  evidence: 'The key goes in x-api-key , x-rapidapi-key , or Authorization: Bearer , whichever your client makes easiest.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a RapidAPI key from RapidAPI (or use the free sign‑in key provided after Google sign‑in).\nnote: No OAuth flows are described on the pages.\ndocs: https://flightpowers.com/mcp\n"
source_yaml_url: https://artifacts.apis.io/flightpowers-com/authentication/flightpowers-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Travel
- Data
- API
- Flights
- Hotels
---
