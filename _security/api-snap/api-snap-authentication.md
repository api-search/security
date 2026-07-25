---
api_key_in: []
api_specs:
- filename: api-snap-browser-api-openapi.yml
  format: yaml
  label: API Snap Browser API
  slug: api-snap-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-browser-api-openapi.yml
- filename: api-snap-documents-api-openapi.yml
  format: yaml
  label: API Snap Documents API
  slug: api-snap-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-documents-api-openapi.yml
- filename: api-snap-images-api-openapi.yml
  format: yaml
  label: API Snap Images API
  slug: api-snap-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-images-api-openapi.yml
- filename: api-snap-security-api-openapi.yml
  format: yaml
  label: API Snap Security API
  slug: api-snap-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-security-api-openapi.yml
- filename: api-snap-utilities-api-openapi.yml
  format: yaml
  label: API Snap Utilities API
  slug: api-snap-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/openapi/api-snap-utilities-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Api Snap Authentication
name_suffix: Authentication
oauth_flows: []
overview: API Snap secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: API Snap
provider_slug: api-snap
scheme_count: 1
schemes:
- description: 'API key obtained from your API Snap dashboard. Pass as `Authorization: Bearer <key>` header or as `?api_key=<key>` query parameter.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/api-snap-openapi.yml
  type: http
slug: api-snap-authentication
source_filename: api-snap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/api-snap-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key obtained from your API Snap dashboard. Pass as `Authorization: Bearer\n    <key>` header or as `?api_key=<key>` query parameter.'\n  sources:\n  - openapi/api-snap-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-snap/refs/heads/main/authentication/api-snap-authentication.yml
summary_line: http · 1 scheme
tags:
- API Utilities
- Developer Tools
- QR Codes
- Screenshots
- Image Processing
- PDF Generation
- Markdown
- URL Metadata
- Hashing
- JWT
- Base64
- UUID
- Color Conversion
- Lorem Ipsum
- Placeholder Images
---
