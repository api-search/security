---
api_key_in: []
api_specs:
- filename: imagekit-account-management-api-api-openapi.yml
  format: yaml
  label: ImageKit Account Management API API
  slug: imagekit-account-management-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-account-management-api-api-openapi.yml
- filename: imagekit-caching-api-openapi.yml
  format: yaml
  label: ImageKit Caching API
  slug: imagekit-caching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-caching-api-openapi.yml
- filename: imagekit-custom-metadata-fields-api-openapi.yml
  format: yaml
  label: ImageKit Custom metadata fields API
  slug: imagekit-custom-metadata-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-custom-metadata-fields-api-openapi.yml
- filename: imagekit-digital-asset-management-dam-api-openapi.yml
  format: yaml
  label: ImageKit Digital Asset Management (DAM) API
  slug: imagekit-digital-asset-management-dam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-digital-asset-management-dam-api-openapi.yml
- filename: imagekit-dummy-test-api-openapi.yml
  format: yaml
  label: ImageKit Dummy Test API
  slug: imagekit-dummy-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-dummy-test-api-openapi.yml
- filename: imagekit-file-metadata-api-openapi.yml
  format: yaml
  label: ImageKit File Metadata API
  slug: imagekit-file-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-file-metadata-api-openapi.yml
- filename: imagekit-managing-assets-api-openapi.yml
  format: yaml
  label: ImageKit Managing assets API
  slug: imagekit-managing-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-managing-assets-api-openapi.yml
- filename: imagekit-managing-folders-api-openapi.yml
  format: yaml
  label: ImageKit Managing folders API
  slug: imagekit-managing-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-managing-folders-api-openapi.yml
- filename: imagekit-origins-api-openapi.yml
  format: yaml
  label: ImageKit Origins API
  slug: imagekit-origins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-origins-api-openapi.yml
- filename: imagekit-saved-extensions-api-openapi.yml
  format: yaml
  label: ImageKit Saved Extensions API
  slug: imagekit-saved-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-saved-extensions-api-openapi.yml
- filename: imagekit-upload-file-api-openapi.yml
  format: yaml
  label: ImageKit Upload File API
  slug: imagekit-upload-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-upload-file-api-openapi.yml
- filename: imagekit-url-endpoints-api-openapi.yml
  format: yaml
  label: ImageKit URL endpoints API
  slug: imagekit-url-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-json-v1-9-imagekit/refs/heads/main/openapi/imagekit-url-endpoints-api-openapi.yml
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
