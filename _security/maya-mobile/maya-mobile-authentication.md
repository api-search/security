---
api_key_in: []
api_specs:
- filename: maya-mobile-openapi.yml
  format: yaml
  label: Maya Mobile Plans and Products API
  slug: plans-products
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-openapi.yml
- filename: maya-mobile-openapi.yml
  format: yaml
  label: Maya Mobile eSIMs and Provisioning API
  slug: esims-provisioning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-openapi.yml
- filename: maya-mobile-openapi.yml
  format: yaml
  label: Maya Mobile Usage and Topup API
  slug: usage-topup
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-openapi.yml
- filename: maya-mobile-openapi.yml
  format: yaml
  label: Maya Mobile Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-openapi.yml
- filename: maya-mobile-openapi.yml
  format: yaml
  label: Maya Mobile Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/openapi/maya-mobile-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Maya Mobile Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maya Mobile secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Maya Mobile
provider_slug: maya-mobile
scheme_count: 1
schemes:
- description: 'Bearer token / API key supplied in the Authorization header (`Authorization: Bearer <token>`). Credentials are issued to onboarded Maya Mobile resellers/partners.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/maya-mobile-openapi.yml
  type: http
slug: maya-mobile-authentication
source_filename: maya-mobile-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/maya-mobile-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token / API key supplied in the Authorization header (`Authorization:\n    Bearer <token>`). Credentials are issued to onboarded Maya Mobile resellers/partners.'\n  sources:\n  - openapi/maya-mobile-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maya-mobile/refs/heads/main/authentication/maya-mobile-authentication.yml
summary_line: http · 1 scheme
tags:
- eSIM
- Connectivity
- Mobile Data
- Roaming
- Telecom
---
