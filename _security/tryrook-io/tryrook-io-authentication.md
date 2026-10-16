---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tryrook-io-openapi-generated.yml
  format: yaml
  label: ROOK API
  slug: tryrook-io-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tryrook-io/refs/heads/main/openapi/_ae-authored/tryrook-io-openapi-generated.yml
auth_types: []
description: Authentication for ROOK API endpoints
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Tryrook Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: ROOK declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ROOK
provider_slug: tryrook-io
scheme_count: 1
schemes:
- evidence: 'Authorization: Basic {Base64Encoded(client_uuid:secret_key)}'
  header: Authorization
  how_to_obtain: Base64‑encode the client_uuid and secret_key separated by a colon and include it in the Authorization header.
  location: header
  name: Basic
  type: http-basic
slug: tryrook-io-authentication
source_filename: tryrook-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.tryrook.io/docs/rookconnect/data-authorization/
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.tryrook.io/docs/rookconnect/data-authorization/\nsources:\n- https://docs.tryrook.io/docs/rookconnect/data-authorization/\n- https://docs.tryrook.io/docs/rookconnect/quickstart/\n- https://docs.tryrook.io/docs/rookscore2.0/QuickStart/\n- https://docs.tryrook.io/docs/rookconnect/quickstart/\ndescription: Authentication for ROOK API endpoints\nschemes:\n- type: http-basic\n  name: Basic\n  evidence: 'Authorization: Basic {Base64Encoded(client_uuid:secret_key)}'\n  location: header\n  header: Authorization\n  how_to_obtain: Base64‑encode the client_uuid and secret_key separated by a colon and include it in the Authorization header.\ndocs: https://docs.tryrook.io/docs/rookconnect/data-authorization/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tryrook-io/refs/heads/main/authentication/tryrook-io-authentication.yml
summary_line: 1 scheme
tags:
- Health
- API
- Data Integration
- Wearables
- Healthcare
---
