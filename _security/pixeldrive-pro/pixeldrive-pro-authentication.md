---
anonymous_access: false
api_key_in: []
auth_types: []
description: PixelDrive uses a simple Bearer token authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Pixeldrive Pro Authentication
name_suffix: Authentication
oauth_flows: []
overview: PixelDrive declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: PixelDrive
provider_slug: pixeldrive-pro
scheme_count: 1
schemes:
- evidence: Authenticate with a Bearer token, POST a template id plus your data, get a PNG URL back.
  header: Authorization
  how_to_obtain: Create a token in your dashboard under API tokens.
  location: header
  name: Bearer token
  type: http-bearer
slug: pixeldrive-pro-authentication
source_filename: pixeldrive-pro-authentication.yml
source_heading: Authentication Profile
source_url: https://pixeldrive.pro/docs
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://pixeldrive.pro/docs\nsources:\n- https://pixeldrive.pro/docs\ndescription: PixelDrive uses a simple Bearer token authentication.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Authenticate with a Bearer token, POST a template id plus your data, get a PNG URL back.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token in your dashboard under API tokens.\nnote: No OAuth2, apiKey, http-basic, jwt, hmac, mtls, or other schemes are documented on the page.\ndocs: https://pixeldrive.pro/docs\n"
source_yaml_url: https://artifacts.apis.io/pixeldrive-pro/authentication/pixeldrive-pro-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Image Generation
- Bulk Rendering
- Marketing
---
