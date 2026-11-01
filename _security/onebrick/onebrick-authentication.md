---
anonymous_access: false
api_key_in: []
api_specs:
- filename: onebrick-openapi-generated.yml
  format: yaml
  label: Brick API
  slug: onebrick-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onebrick/openapi/_ae-authored/onebrick-openapi-generated.yml
auth_types: []
description: Brick APIs use short-lived, one-time public access tokens for API authentication. Each token is valid for a single request and expires within 5 minutes of generation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Onebrick Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brick declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Brick
provider_slug: onebrick
scheme_count: 1
schemes:
- evidence: Brick APIs use short-lived, one-time public access tokens for API authentication. Each token is valid for a single request and expires within 5 minutes of generation.
  header: publicAccessToken
  how_to_obtain: Generate a new public access token immediately before each API request via the Brick Dashboard’s API Credentials section.
  location: header
  name: publicAccessToken
  type: apiKey
slug: onebrick-authentication
source_filename: onebrick-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.onebrick.io/getting-started/authentication-and-environment
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.onebrick.io/getting-started/authentication-and-environment\nsources:\n- https://docs.onebrick.io/getting-started/authentication-and-environment\n- https://docs.onebrick.io/th/getting-started/authentication-and-environment\n- https://docs.onebrick.io/id/getting-started/authentication-and-environment\n- https://docs.onebrick.io/getting-started/subaccount-management/b2c-client-regenerate-api-key\ndescription: Brick APIs use short-lived, one-time public access tokens for API authentication. Each token is valid for a single request and expires\n  within 5 minutes of generation.\nschemes:\n- type: apiKey\n  name: publicAccessToken\n  evidence: Brick APIs use short-lived, one-time public access tokens for API authentication. Each token is valid for a single request and expires\n    within 5 minutes of generation.\n  location: header\n  header: publicAccessToken\n  how_to_obtain:\
  \ Generate a new public access token immediately before each API request via the Brick Dashboard’s API Credentials section.\nnote: QR Code SNAP APIs use a separate SNAP B2B access token flow, which is not described on these pages.\ndocs: https://docs.onebrick.io/getting-started/authentication-and-environment\n"
source_yaml_url: https://artifacts.apis.io/onebrick/authentication/onebrick-authentication.yml
summary_line: 1 scheme
tags:
- Fintech
- Payments
- Southeast Asia
- B2B
---
