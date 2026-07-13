---
api_key_in: []
api_specs:
- filename: itsacheckmate-marketplace-api.yml
  format: yaml
  label: Marketplace for Developers API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/itsacheckmate/refs/heads/main/openapi/itsacheckmate-marketplace-api.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Itsacheckmate Authentication
name_suffix: Authentication
oauth_flows: []
overview: ItsaCheckmate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ItsaCheckmate
provider_slug: itsacheckmate
scheme_count: 1
schemes:
- description: OAuth-style scoped access token issued by /oauth/token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/itsacheckmate-marketplace-api.yml
  type: http
slug: itsacheckmate-authentication
source_filename: itsacheckmate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/itsacheckmate-marketplace-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth-style scoped access token issued by /oauth/token.\n  sources:\n  - openapi/itsacheckmate-marketplace-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itsacheckmate/refs/heads/main/authentication/itsacheckmate-authentication.yml
summary_line: http · 1 scheme
tags:
- Restaurant
- Point Of Sale
- Online Ordering
- Delivery
- Menus
- Orders
- Integration
---
