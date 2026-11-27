---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mapsource-io-account-api-openapi.yml
  format: yaml
  label: Mapsource Account API
  slug: mapsource-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-account-api-openapi.yml
- filename: mapsource-io-cartography-api-openapi.yml
  format: yaml
  label: Mapsource Cartography API
  slug: mapsource-io-cartography-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-cartography-api-openapi.yml
- filename: mapsource-io-compute-api-openapi.yml
  format: yaml
  label: Mapsource Compute API
  slug: mapsource-io-compute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-compute-api-openapi.yml
- filename: mapsource-io-delivery-api-openapi.yml
  format: yaml
  label: Mapsource Delivery API
  slug: mapsource-io-delivery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-delivery-api-openapi.yml
- filename: mapsource-io-discovery-api-openapi.yml
  format: yaml
  label: Mapsource Discovery API
  slug: mapsource-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-discovery-api-openapi.yml
- filename: mapsource-io-meta-api-openapi.yml
  format: yaml
  label: Mapsource Meta API
  slug: mapsource-io-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-meta-api-openapi.yml
- filename: mapsource-io-navigation-api-openapi.yml
  format: yaml
  label: Mapsource Navigation API
  slug: mapsource-io-navigation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-navigation-api-openapi.yml
- filename: mapsource-io-terrain-api-openapi.yml
  format: yaml
  label: Mapsource Terrain API
  slug: mapsource-io-terrain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-terrain-api-openapi.yml
- filename: mapsource-io-weather-api-openapi.yml
  format: yaml
  label: Mapsource Weather API
  slug: mapsource-io-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-weather-api-openapi.yml
auth_types: []
description: Mapsources uses API keys as Bearer tokens in the Authorization header, and also supports legacy key placement in the URL path or query string.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Mapsource Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mapsource declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Mapsource
provider_slug: mapsource-io
scheme_count: 3
schemes:
- evidence: 'Authenticated endpoints require an Authorization: Bearer $MAPSOURCE_API_KEY header.'
  header: Authorization
  how_to_obtain: Obtain a key from the pricing page after account verification; the key is displayed once on the completion page.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: The interpreter also accepts legacy path and query credentials for compatible clients; the client guide documents the exact routes and their limitations.
  how_to_obtain: Obtain a key from the pricing page after account verification; the key is displayed once on the completion page.
  location: path
  name: Legacy path key
  type: apiKey
- evidence: Legacy query /interpreter?key={key} Also accepts api_key; exposes the key in the URL.
  how_to_obtain: Obtain a key from the pricing page after account verification; the key is displayed once on the completion page.
  location: query
  name: Legacy query key
  type: apiKey
slug: mapsource-io-authentication
source_filename: mapsource-io-authentication.yml
source_heading: Authentication Profile
source_url: https://mapsource.io/docs/reference
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mapsource.io/docs/reference\nsources:\n- https://mapsource.io/docs/reference\n- https://mapsource.io/docs/usage\n- https://mapsource.io/docs/quickstart\n- https://mapsource.io/docs/clients\ndescription: Mapsources uses API keys as Bearer tokens in the Authorization header, and also supports legacy key placement in the URL path or\n  query string.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Authenticated endpoints require an Authorization: Bearer $MAPSOURCE_API_KEY header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a key from the pricing page after account verification; the key is displayed once on the completion page.\n- type: apiKey\n  name: Legacy path key\n  evidence: The interpreter also accepts legacy path and query credentials for compatible clients; the client guide documents the exact routes\n    and their limitations.\n\
  \  location: path\n  how_to_obtain: Obtain a key from the pricing page after account verification; the key is displayed once on the completion page.\n- type: apiKey\n  name: Legacy query key\n  evidence: Legacy query /interpreter?key={key} Also accepts api_key; exposes the key in the URL.\n  location: query\n  how_to_obtain: Obtain a key from the pricing page after account verification; the key is displayed once on the completion page.\nnote: No OAuth2, JWT, HMAC, MTLS, or other schemes are documented.\ndocs: https://mapsource.io/docs/reference\n"
source_yaml_url: https://artifacts.apis.io/mapsource-io/authentication/mapsource-io-authentication.yml
summary_line: 3 schemes
tags:
- Geospatial
- OpenStreetMap
- Mapping
- Cloud
---
