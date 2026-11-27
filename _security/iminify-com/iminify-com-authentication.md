---
anonymous_access: false
api_key_in: []
api_specs:
- filename: iminify-com-openapi-generated.yml
  format: yaml
  label: Iminify API
  slug: iminify-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iminify-com/openapi/_ae-authored/iminify-com-openapi-generated.yml
auth_types: []
description: Iminify API authentication uses a personal access token (API key) sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Iminify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Iminify declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Iminify
provider_slug: iminify-com
scheme_count: 1
schemes:
- evidence: 'Put the key in the Authorization header as a Bearer token, on every request:'
  header: Authorization
  how_to_obtain: Create an API key in Settings > API Tokens, then copy the key.
  location: header
  name: Bearer
  type: http-bearer
slug: iminify-com-authentication
source_filename: iminify-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.iminify.com/docs/authentication
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.iminify.com/docs/authentication\nsources:\n- https://www.iminify.com/docs/authentication\n- https://www.iminify.com/blog/19-does-compression-remove-content-credentials-two-signed-gemini-images-through-13-tools\n- https://www.iminify.com/blog/17-how-many-tokens-is-an-image-claude-gpt-and-gemini-measured-on-seven-real-files\ndescription: Iminify API authentication uses a personal access token (API key) sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Put the key in the Authorization header as a Bearer token, on every request:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings > API Tokens, then copy the key.\ndocs: https://www.iminify.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/iminify-com/authentication/iminify-com-authentication.yml
summary_line: 1 scheme
tags:
- Image Compression
- Free
- Online Tool
- Formats
---
