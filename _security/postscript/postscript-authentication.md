---
api_key_in: []
api_specs:
- filename: postscript-events-api-openapi.yml
  format: yaml
  label: Postscript Events API
  slug: postscript-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-events-api-openapi.yml
- filename: postscript-subscribers-api-openapi.yml
  format: yaml
  label: Postscript Subscribers API
  slug: postscript-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-subscribers-api-openapi.yml
- filename: postscript-webhooks-api-openapi.yml
  format: yaml
  label: Postscript Webhooks API
  slug: postscript-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Postscript Authentication
name_suffix: Authentication
oauth_flows: []
overview: Postscript secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Postscript
provider_slug: postscript
scheme_count: 1
schemes:
- description: 'Postscript uses bearer token authentication. Generate API keys from the

    Postscript app under API Settings.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/postscript-openapi.yml
  type: http
slug: postscript-authentication
source_filename: postscript-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/postscript-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Postscript uses bearer token authentication. Generate API keys from the\n    Postscript app under API Settings.\n  sources:\n  - openapi/postscript-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/authentication/postscript-authentication.yml
summary_line: http · 1 scheme
tags:
- SMS
- Marketing
- Messaging
- E-commerce
- Shopify
- RCS
- Subscribers
---
