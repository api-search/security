---
api_key_in: []
api_specs:
- filename: cloudinary-openapi.yml
  format: yaml
  label: Cloudinary Upload API
  slug: upload
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudinary/refs/heads/main/openapi/cloudinary-openapi.yml
- filename: cloudinary-notifications-asyncapi.yml
  format: yaml
  label: Cloudinary Notifications and Webhooks
  slug: notifications
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudinary/refs/heads/main/asyncapi/cloudinary-notifications-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cloudinary Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudinary secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cloudinary
provider_slug: cloudinary
scheme_count: 1
schemes:
- description: HTTP Basic auth using API key as username and API secret as password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/cloudinary-openapi.yml
  type: http
slug: cloudinary-authentication
source_filename: cloudinary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudinary-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using API key as username and API secret as password.\n  sources:\n  - openapi/cloudinary-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudinary/refs/heads/main/authentication/cloudinary-authentication.yml
summary_line: http · 1 scheme
tags:
- Asset Management
- Digital Asset Management
- Image Processing
- Image Transformation
- Media
- SaaS
- Video Processing
---
