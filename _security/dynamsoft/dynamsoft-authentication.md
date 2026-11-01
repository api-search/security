---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for Dynamic Web TWAIN Service
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dynamsoft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dynamsoft Web TWAIN declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dynamsoft Web TWAIN
provider_slug: dynamsoft
scheme_count: 1
schemes:
- evidence: Using the REST API, you need to set the header to use the token.
  header: Authorization
  how_to_obtain: 'Generate a token with the command: "C:\Program Files (x86)\Dynamsoft\Dynamic Web TWAIN Service 19\DynamicWebTWAINService.exe" Config --create-token "{\"duration\":864000}"'
  location: header
  name: Bearer token
  type: http-bearer
slug: dynamsoft-authentication
source_filename: dynamsoft-authentication.yml
source_heading: Authentication Profile
source_url: https://www.dynamsoft.com/web-twain/docs/extended-usage/access-token.html
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.dynamsoft.com/web-twain/docs/extended-usage/access-token.html\nsources:\n- https://www.dynamsoft.com/web-twain/docs/extended-usage/access-token.html\ndescription: Authentication for Dynamic Web TWAIN Service\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Using the REST API, you need to set the header to use the token.\n  location: header\n  header: Authorization\n  how_to_obtain: 'Generate a token with the command: \"C:\\Program Files (x86)\\Dynamsoft\\Dynamic Web TWAIN Service 19\\DynamicWebTWAINService.exe\"\n    Config --create-token \"{\\\"duration\\\":864000}\"'\ndocs: https://www.dynamsoft.com/web-twain/docs/extended-usage/access-token.html\n"
source_yaml_url: https://artifacts.apis.io/dynamsoft/authentication/dynamsoft-authentication.yml
summary_line: 1 scheme
tags:
- Company
- SDK
- Document-Capture
- Barcode
- MRZ
- Web
---
