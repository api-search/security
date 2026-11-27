---
anonymous_access: true
api_key_in: []
api_specs:
- filename: corkandcurve-com-bookable-api-openapi.yml
  format: yaml
  label: Cork & Curve Bookable API
  slug: corkandcurve-com-bookable-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corkandcurve-com/openapi/corkandcurve-com-bookable-api-openapi.yml
- filename: corkandcurve-com-festivals-api-openapi.yml
  format: yaml
  label: Cork & Curve Festivals API
  slug: corkandcurve-com-festivals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corkandcurve-com/openapi/corkandcurve-com-festivals-api-openapi.yml
- filename: corkandcurve-com-meta-api-openapi.yml
  format: yaml
  label: Cork & Curve Meta API
  slug: corkandcurve-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corkandcurve-com/openapi/corkandcurve-com-meta-api-openapi.yml
- filename: corkandcurve-com-places-api-openapi.yml
  format: yaml
  label: Cork & Curve Places API
  slug: corkandcurve-com-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corkandcurve-com/openapi/corkandcurve-com-places-api-openapi.yml
- filename: corkandcurve-com-site-api-openapi.yml
  format: yaml
  label: Cork & Curve Site API
  slug: corkandcurve-com-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corkandcurve-com/openapi/corkandcurve-com-site-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cork & Curve Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cork & Curve declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cork & Curve
provider_slug: corkandcurve-com
scheme_count: 2
schemes:
- description: No key is needed. Every request is counted against a per-IP limit (120 a minute); a refused request gets HTTP 429 with Retry-After.
  name: anonymous
  type: none
- alternate:
    in: query
    name: api_key
  description: A key gives your agent its own attribution tag on the booking links it hands out and its own rate limit. Send it as the `X-API-Key` header (or the `api_key` query parameter).
  in: header
  issuance: Keys are issued by us on request through https://corkandcurve.com/contact/ ; there is no self-serve sign-up.
  name: X-API-Key
  required: false
  type: apiKey
slug: corkandcurve-com-authentication
source_filename: corkandcurve-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://corkandcurve.com/auth.md\ndocs: https://corkandcurve.com/auth.md\nname: Cork & Curve authentication\nsummary: No sign-in and no OAuth. The REST API and the MCP server are public; an optional API key adds attribution and its own rate limit.\nschemes:\n- type: none\n  name: anonymous\n  description: \"No key is needed. Every request is counted against a per-IP limit (120 a minute); a refused request gets HTTP 429 with Retry-After.\"\n- type: apiKey\n  name: X-API-Key\n  in: header\n  required: false\n  alternate: {in: query, name: api_key}\n  description: \"A key gives your agent its own attribution tag on the booking links it hands out and its own rate limit. Send it as the `X-API-Key` header (or the `api_key` query parameter).\"\n  issuance: \"Keys are issued by us on request through https://corkandcurve.com/contact/ ; there is no self-serve sign-up.\"\noauth: false\nnote: The OpenAPI declares no securitySchemes; the\
  \ optional key appears only as per-operation x-api-key header and api_key query parameters.\n"
source_yaml_url: https://artifacts.apis.io/corkandcurve-com/authentication/corkandcurve-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Wine
- Travel
- Travel Guides
- Publishing
- Food and Beverage
- MCP
---
