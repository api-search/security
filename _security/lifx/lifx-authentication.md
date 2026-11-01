---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lifx-color-api-openapi.yml
  format: yaml
  label: LIFX Color API
  slug: lifx-color-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lifx/openapi/lifx-color-api-openapi.yml
- filename: lifx-lights-api-openapi.yml
  format: yaml
  label: LIFX Lights API
  slug: lifx-lights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lifx/openapi/lifx-lights-api-openapi.yml
- filename: lifx-scenes-api-openapi.yml
  format: yaml
  label: LIFX Scenes API
  slug: lifx-scenes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lifx/openapi/lifx-scenes-api-openapi.yml
auth_types: []
description: All requests require an OAuth 2 access token. Authenticate with HTTP Basic Authentication or the HTTP Authorization header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lifx Authentication
name_suffix: Authentication
oauth_flows: []
overview: LIFX declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LIFX
provider_slug: lifx
scheme_count: 2
schemes:
- evidence: Authenticate with HTTP Basic Authentication or the HTTP Authorization header.
  header: Authorization
  how_to_obtain: Generate an access token in your account settings.
  location: header
  name: Authorization Header
  type: http-bearer
- evidence: When using HTTP Basic Authentication the access token is the username and the password may be left blank.
  header: Authorization
  how_to_obtain: Generate an access token in your account settings.
  location: header
  name: Basic Authentication
  type: http-basic
slug: lifx-authentication
source_filename: lifx-authentication.yml
source_heading: Authentication Profile
source_url: https://api.developer.lifx.com/reference/authentication.md
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.developer.lifx.com/reference/authentication.md\nsources:\n- https://api.developer.lifx.com/reference/authentication.md\n- https://api.developer.lifx.com/reference/authentication\ndescription: All requests require an OAuth 2 access token. Authenticate with HTTP Basic Authentication or the HTTP Authorization header.\nschemes:\n- type: http-bearer\n  name: Authorization Header\n  evidence: Authenticate with HTTP Basic Authentication or the HTTP Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an access token in your account settings.\n- type: http-basic\n  name: Basic Authentication\n  evidence: When using HTTP Basic Authentication the access token is the username and the password may be left blank.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an access token in your account settings.\nnote: OAuth flow\
  \ URLs and scopes are not provided on the page.\ndocs: https://api.developer.lifx.com/reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/lifx/authentication/lifx-authentication.yml
summary_line: 2 schemes
tags:
- Smart Lighting
- Wi‑Fi Bulbs
- Home Automation
- Lighting Fixtures
---
