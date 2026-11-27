---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openqr-uk-me-api-openapi.yml
  format: yaml
  label: OpenQR Me API
  slug: openqr-uk-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openqr-uk/openapi/openqr-uk-me-api-openapi.yml
- filename: openqr-uk-openqr-api-api-openapi.yml
  format: yaml
  label: OpenQR OpenQR API
  slug: openqr-uk-openqr-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openqr-uk/openapi/openqr-uk-openqr-api-api-openapi.yml
auth_types: []
description: OpenQR API uses a bearer token passed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: OpenQR Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenQR declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OpenQR
provider_slug: openqr-uk
scheme_count: 1
schemes:
- evidence: Keys look like oqr_… and travel as a bearer token.
  header: Authorization
  how_to_obtain: Go to openqr.uk/api, sign in with a magic link, then create a key under the dashboard. The key is shown once and stored as a SHA‑256 hash.
  location: header
  name: Bearer
  type: http-bearer
slug: openqr-uk-authentication
source_filename: openqr-uk-authentication.yml
source_heading: Authentication Profile
source_url: https://openqr.uk/blog/qr-code-api-getting-started
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://openqr.uk/blog/qr-code-api-getting-started\nsources:\n- https://openqr.uk/blog/qr-code-api-getting-started\ndescription: OpenQR API uses a bearer token passed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Keys look like oqr_… and travel as a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Go to openqr.uk/api, sign in with a magic link, then create a key under the dashboard. The key is shown once and stored as a\n    SHA‑256 hash.\ndocs: https://openqr.uk/blog/qr-code-api-getting-started\n"
source_yaml_url: https://artifacts.apis.io/openqr-uk/authentication/openqr-uk-authentication.yml
summary_line: 1 scheme
tags:
- QR Codes
- Generator
- Analytics
- BusinessTools
- Open Source
---
