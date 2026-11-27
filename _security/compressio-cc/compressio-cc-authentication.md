---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CompressIO Authentication
name_suffix: Authentication
oauth_flows: []
overview: CompressIO declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CompressIO
provider_slug: compressio-cc
scheme_count: 2
schemes:
- description: 'The API root page''s REST example sends -H "Authorization: Bearer YOUR_KEY". Keys are obtained from the provider''s Ko-fi shop (https://ko-fi.com/yugutou/shop); the page says "API keys at Ko-fi".'
  header: Authorization
  in: header
  name: bearerApiKey
  scheme: bearer
  type: http
- description: 'Anonymous use is allowed without a key, limited per IP ("Anonymous: 20 images/day per IP, max 10MB").'
  name: anonymous
  type: none
slug: compressio-cc-authentication
source_filename: compressio-cc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: CompressIO authentication\ngenerated: '2026-11-04'\nmethod: searched\nsource: https://api.compressio.cc/\ndocs: https://api.compressio.cc/\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: 'The API root page''s REST example sends -H \"Authorization: Bearer YOUR_KEY\". Keys are obtained from the provider''s Ko-fi shop (https://ko-fi.com/yugutou/shop); the page says \"API keys at Ko-fi\".'\n- name: anonymous\n  type: none\n  description: 'Anonymous use is allowed without a key, limited per IP (\"Anonymous: 20 images/day per IP, max 10MB\").'\nnote: No OpenAPI is published (/openapi.json returned 404), so this profile is read from the single docs page, not derived from securitySchemes. No OAuth is documented.\n"
source_yaml_url: https://artifacts.apis.io/compressio-cc/authentication/compressio-cc-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Image Compression
- Image Conversion
- Image Processing
- MCP
- AI Agents
- WebAssembly
---
