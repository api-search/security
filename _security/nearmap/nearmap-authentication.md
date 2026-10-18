---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nearmap-coverage-api-openapi.yml
  format: yaml
  label: Nearmap Coverage API
  slug: nearmap-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nearmap/refs/heads/main/openapi/nearmap-coverage-api-openapi.yml
- filename: nearmap-tiles-api-openapi.yml
  format: yaml
  label: Nearmap Tiles API
  slug: nearmap-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nearmap/refs/heads/main/openapi/nearmap-tiles-api-openapi.yml
auth_types: []
description: Nearmap uses API Key authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nearmap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nearmap declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Nearmap
provider_slug: nearmap
scheme_count: 1
schemes:
- evidence: The API key can be sent with the request using the apikey URL parameter or an HTTP Authorization header.
  how_to_obtain: As a Nearmap user, you can create your own API key in MyAccount.
  location: query
  name: apikey
  type: apiKey
slug: nearmap-authentication
source_filename: nearmap-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.nearmap.com/docs/authentication.md
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.nearmap.com/docs/authentication.md\nsources:\n- https://developer.nearmap.com/docs/authentication.md\n- https://developer.nearmap.com/docs/use-an-api-key-in-nearmap-integrations.md\n- https://developer.nearmap.com/docs/troubleshoot-api-keys.md\n- https://developer.nearmap.com/docs/authentication\ndescription: Nearmap uses API Key authentication.\nschemes:\n- type: apiKey\n  name: apikey\n  evidence: The API key can be sent with the request using the apikey URL parameter or an HTTP Authorization header.\n  location: query\n  how_to_obtain: As a Nearmap user, you can create your own API key in MyAccount.\nnote: No OAuth flows are documented for Nearmap. 1 extracted row(s) were dropped because their quote was not on the page.\ndocs: https://developer.nearmap.com/docs/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nearmap/refs/heads/main/authentication/nearmap-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AerialImagery
- Geospatial
- PropertyIntelligence
---
