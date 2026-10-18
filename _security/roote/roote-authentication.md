---
anonymous_access: false
api_key_in: []
api_specs:
- filename: roote-capabilities-api-openapi.yml
  format: yaml
  label: ROOTE Capabilities API
  slug: roote-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-capabilities-api-openapi.yml
- filename: roote-changelog-json-api-openapi.yml
  format: yaml
  label: ROOTE Changelog.json API
  slug: roote-changelog-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-changelog-json-api-openapi.yml
- filename: roote-charging-api-openapi.yml
  format: yaml
  label: ROOTE Charging API
  slug: roote-charging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-charging-api-openapi.yml
- filename: roote-geocode-api-openapi.yml
  format: yaml
  label: ROOTE Geocode API
  slug: roote-geocode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-geocode-api-openapi.yml
- filename: roote-health-api-openapi.yml
  format: yaml
  label: ROOTE Health API
  slug: roote-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-health-api-openapi.yml
- filename: roote-mobility-api-openapi.yml
  format: yaml
  label: ROOTE Mobility API
  slug: roote-mobility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-mobility-api-openapi.yml
- filename: roote-nearby-api-openapi.yml
  format: yaml
  label: ROOTE Nearby API
  slug: roote-nearby-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-nearby-api-openapi.yml
- filename: roote-openapi-json-api-openapi.yml
  format: yaml
  label: ROOTE Openapi.json API
  slug: roote-openapi-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-openapi-json-api-openapi.yml
- filename: roote-parking-api-openapi.yml
  format: yaml
  label: ROOTE Parking API
  slug: roote-parking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-parking-api-openapi.yml
- filename: roote-place-search-api-openapi.yml
  format: yaml
  label: ROOTE Place Search API
  slug: roote-place-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-place-search-api-openapi.yml
- filename: roote-reverse-geocode-api-openapi.yml
  format: yaml
  label: ROOTE Reverse Geocode API
  slug: roote-reverse-geocode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-reverse-geocode-api-openapi.yml
- filename: roote-ride-hailing-api-openapi.yml
  format: yaml
  label: ROOTE Ride Hailing API
  slug: roote-ride-hailing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-ride-hailing-api-openapi.yml
- filename: roote-services-api-openapi.yml
  format: yaml
  label: ROOTE Services API
  slug: roote-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-services-api-openapi.yml
- filename: roote-transit-api-openapi.yml
  format: yaml
  label: ROOTE Transit API
  slug: roote-transit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-transit-api-openapi.yml
- filename: roote-usage-api-openapi.yml
  format: yaml
  label: ROOTE Usage API
  slug: roote-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-usage-api-openapi.yml
auth_types: []
description: Authentication schemes for ROOTE API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Roote Authentication
name_suffix: Authentication
oauth_flows: []
overview: ROOTE declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ROOTE
provider_slug: roote
scheme_count: 1
schemes:
- evidence: Endpoints that explicitly support query authentication may also accept ?token=YOUR_API_TOKEN
  how_to_obtain: Create and manage developer access at dev.roote.ai and obtain an API token.
  location: query
  name: Bearer token in query
  scopes:
  - data:read
  - journey:read
  type: apiKey
slug: roote-authentication
source_filename: roote-authentication.yml
source_heading: Authentication Profile
source_url: https://doc.roote.ai/authentication
source_yaml: "generated: '2026-10-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://doc.roote.ai/authentication\nsources:\n- https://doc.roote.ai/authentication\n- https://doc.roote.ai/roote-api/api-authentication\n- https://doc.roote.ai/getting-started\ndescription: Authentication schemes for ROOTE API\nschemes:\n- type: apiKey\n  name: Bearer token in query\n  evidence: Endpoints that explicitly support query authentication may also accept ?token=YOUR_API_TOKEN\n  location: query\n  scopes:\n  - data:read\n  - journey:read\n  how_to_obtain: Create and manage developer access at dev.roote.ai and obtain an API token.\nnote: No OAuth2, http-basic, jwt, hmac, mtls, or other schemes are documented. 1 extracted row(s) were dropped because their quote was not on\n  the page.\ndocs: https://doc.roote.ai/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/authentication/roote-authentication.yml
summary_line: 1 scheme
tags:
- Mobility
- French
- Artificial Intelligence
- Transportation
---
