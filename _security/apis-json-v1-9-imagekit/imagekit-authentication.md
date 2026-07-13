---
api_key_in: []
api_specs:
- filename: imagekit-media-api-openapi.yml
  format: yaml
  label: ImageKit Media API
  slug: apis-json-v1-9-imagekit-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imagekit/refs/heads/main/openapi/imagekit-media-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Imagekit Authentication
name_suffix: Authentication
oauth_flows: []
overview: ImageKit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ImageKit
provider_slug: apis-json-v1-9-imagekit
scheme_count: 1
schemes:
- description: 'Basic HTTP authentication. Allowed headers-- Authorization: Basic <private_api_key> | Authorization: Basic <base64 hash of `private_api_key:`>

    ImageKit API uses API keys to authenticate requests. You can view and manage your API keys in [the dashboard](https://imagekit.io/dashboard/developer/api-keys).

    All API requests must be made over HTTPS. Calls made over plain HTTP will fail. API requests wit'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/imagekit-media-api-openapi.yml
  type: http
slug: imagekit-authentication
source_filename: imagekit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/imagekit-media-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Basic HTTP authentication. Allowed headers-- Authorization: Basic <private_api_key> | Authorization: Basic <base64 hash of `private_api_key:`>\n    ImageKit API uses API keys to authenticate requests. You can view and manage your API keys in [the dashboard](https://imagekit.io/dashboard/developer/api-keys).\n    All API requests must be made over HTTPS. Calls made over plain HTTP will fail. API requests wit\n  sources:\n  - openapi/imagekit-media-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/authentication/imagekit-authentication.yml
summary_line: http · 1 scheme
tags:
- Images
- Video
- CDN
- Media
- Optimization
- Transformations
- Digital Asset Management
- DAM
- Storage
- Cache
- Upload
---
