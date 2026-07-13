---
api_key_in: []
api_specs:
- filename: bytescale-openapi.yml
  format: yaml
  label: Bytescale File Upload API
  slug: bytescale-file-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytescale/refs/heads/main/openapi/bytescale-openapi.yml
- filename: bytescale-openapi.yml
  format: yaml
  label: Bytescale Files Management API
  slug: bytescale-files-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytescale/refs/heads/main/openapi/bytescale-openapi.yml
- filename: bytescale-openapi.yml
  format: yaml
  label: Bytescale Image / Video Processing API
  slug: bytescale-image-video-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytescale/refs/heads/main/openapi/bytescale-openapi.yml
- filename: bytescale-openapi.yml
  format: yaml
  label: Bytescale CDN / Serving API
  slug: bytescale-cdn-serving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bytescale/refs/heads/main/openapi/bytescale-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bytescale Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bytescale secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bytescale
provider_slug: bytescale
scheme_count: 1
schemes:
- description: Bytescale API key passed as a Bearer token. Secret keys (secret_*) are required for write and management operations; public keys (public_*) may be used with JWT-based auth.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bytescale-openapi.yml
  type: http
slug: bytescale-authentication
source_filename: bytescale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bytescale-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bytescale API key passed as a Bearer token. Secret keys (secret_*) are required\n    for write and management operations; public keys (public_*) may be used with JWT-based auth.\n  sources:\n  - openapi/bytescale-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bytescale/refs/heads/main/authentication/bytescale-authentication.yml
summary_line: http · 1 scheme
tags:
- File Upload
- Storage
- Image Processing
- CDN
- Media
---
