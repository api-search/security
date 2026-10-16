---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eagleview-order-adjustments-api-openapi.yml
  format: yaml
  label: EagleView Order Adjustments API
  slug: eagleview-order-adjustments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eagleview/refs/heads/main/openapi/eagleview-order-adjustments-api-openapi.yml
- filename: eagleview-order-status-api-openapi.yml
  format: yaml
  label: EagleView Order Status API
  slug: eagleview-order-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eagleview/refs/heads/main/openapi/eagleview-order-status-api-openapi.yml
- filename: eagleview-ordering-api-openapi.yml
  format: yaml
  label: EagleView Ordering API
  slug: eagleview-ordering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eagleview/refs/heads/main/openapi/eagleview-ordering-api-openapi.yml
- filename: eagleview-retrieving-files-api-openapi.yml
  format: yaml
  label: EagleView Retrieving Files API
  slug: eagleview-retrieving-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eagleview/refs/heads/main/openapi/eagleview-retrieving-files-api-openapi.yml
auth_types: []
description: Eagleview supports OAuth 2.0 and API key authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Eagleview Authentication
name_suffix: Authentication
oauth_flows: []
overview: EagleView declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: EagleView
provider_slug: eagleview
scheme_count: 1
schemes:
- evidence: Include your key in the request header or query string.
  how_to_obtain: An API key provided via the Eagleview developer portal.
  location: header or query
  name: Eagleview API Key
  type: apiKey
slug: eagleview-authentication
source_filename: eagleview-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.eagleview.com/docs/authentication/overview.md
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.eagleview.com/docs/authentication/overview.md\nsources:\n- https://developer.eagleview.com/docs/authentication/overview.md\n- https://developer.eagleview.com/docs/authentication/client-credentials.md\n- https://developer.eagleview.com/docs/authentication/authorization-code.md\n- https://developer.eagleview.com/docs/authentication/authorization-with-pkce.md\ndescription: Eagleview supports OAuth 2.0 and API key authentication.\nschemes:\n- type: apiKey\n  name: Eagleview API Key\n  evidence: Include your key in the request header or query string.\n  location: header or query\n  how_to_obtain: An API key provided via the Eagleview developer portal.\ndocs: https://developer.eagleview.com/docs/authentication/overview.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eagleview/refs/heads/main/authentication/eagleview-authentication.yml
summary_line: 1 scheme
tags:
- Geospatial
- AerialImagery
- DataAnalytics
- RealEstate
- Insurance
---
