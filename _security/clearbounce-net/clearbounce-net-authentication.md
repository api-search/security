---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clearbounce-net-openapi-generated.yml
  format: yaml
  label: ClearBounce API
  slug: clearbounce-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearbounce-net/openapi/_ae-authored/clearbounce-net-openapi-generated.yml
auth_types: []
description: ClearBounce uses a simple API key authentication scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Clearbounce Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClearBounce declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ClearBounce
provider_slug: clearbounce-net
scheme_count: 1
schemes:
- evidence: 'All API requests must include your API key in the X-API-Key header:'
  header: X-API-Key
  how_to_obtain: Log in to your ClearBounce Dashboard → Navigate to the API section → Your API key is displayed there → Click "Copy" to copy it to your clipboard.
  location: header
  name: ClearBounce API Key
  type: apiKey
slug: clearbounce-net-authentication
source_filename: clearbounce-net-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.clearbounce.net/api-reference/authentication
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.clearbounce.net/api-reference/authentication\nsources:\n- https://docs.clearbounce.net/api-reference/authentication\n- https://docs.clearbounce.net/quick-start\ndescription: ClearBounce uses a simple API key authentication scheme.\nschemes:\n- type: apiKey\n  name: ClearBounce API Key\n  evidence: 'All API requests must include your API key in the X-API-Key header:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Log in to your ClearBounce Dashboard → Navigate to the API section → Your API key is displayed there → Click \"Copy\" to copy it\n    to your clipboard.\nnote: API Key Management endpoints require JWT authentication, but the primary API calls use the X-API-Key header as described.\ndocs: https://docs.clearbounce.net/api-reference/authentication\n"
source_yaml_url: https://artifacts.apis.io/clearbounce-net/authentication/clearbounce-net-authentication.yml
summary_line: 1 scheme
tags:
- Email Verification
- List Cleaning
- Form Validation
- Deliverability
- Marketing Tools
- Enterprise Solutions
---
