---
anonymous_access: false
api_key_in: []
api_specs:
- filename: echelongraph-io-openapi-generated.yml
  format: yaml
  label: EchelonGraph API
  slug: echelongraph-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/echelongraph-io/openapi/_ae-authored/echelongraph-io-openapi-generated.yml
auth_types: []
description: Authentication schemes as published on the page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Echelongraph Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: EchelonGraph declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: EchelonGraph
provider_slug: echelongraph-io
scheme_count: 1
schemes:
- evidence: All API requests require a valid bearer token. Authenticate via the login endpoint to receive an access token and refresh token pair.
  header: Authorization
  how_to_obtain: login endpoint
  location: header
  name: Bearer
  type: http-bearer
slug: echelongraph-io-authentication
source_filename: echelongraph-io-authentication.yml
source_heading: Authentication Profile
source_url: https://echelongraph.io/docs/api-reference
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://echelongraph.io/docs/api-reference\nsources:\n- https://echelongraph.io/docs/api-reference\n- https://echelongraph.io/docs/getting-started\n- https://echelongraph.io/docs/integrations\ndescription: Authentication schemes as published on the page.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: All API requests require a valid bearer token. Authenticate via the login endpoint to receive an access token and refresh token pair.\n  location: header\n  header: Authorization\n  how_to_obtain: login endpoint\ndocs: https://echelongraph.io/docs/api-reference\n"
source_yaml_url: https://artifacts.apis.io/echelongraph-io/authentication/echelongraph-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Cloud
- Security
- Compliance
- Monitoring
---
