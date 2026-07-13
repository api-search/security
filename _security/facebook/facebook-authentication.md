---
api_key_in: []
api_specs:
- filename: facebook-graph-api.yaml
  format: yaml
  label: Facebook Graph API
  slug: facebook-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-graph-api.yaml
- filename: facebook-marketing-api.yaml
  format: yaml
  label: Facebook Marketing API
  slug: facebook-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-marketing-api.yaml
- filename: facebook-instagram-api.yaml
  format: yaml
  label: Instagram API
  slug: instagram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-instagram-api.yaml
- filename: facebook-messenger-api.yaml
  format: yaml
  label: Messenger Platform API
  slug: messenger-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-messenger-api.yaml
- filename: facebook-threads-api.yaml
  format: yaml
  label: Threads API
  slug: threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-threads-api.yaml
- filename: facebook-whatsapp-api.yaml
  format: yaml
  label: WhatsApp Business API
  slug: whatsapp-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-whatsapp-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Facebook Authentication
name_suffix: Authentication
oauth_flows: []
overview: Facebook secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Facebook
provider_slug: facebook
scheme_count: 1
schemes:
- description: OAuth 2.0 access token for Facebook Graph API.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/facebook-graph-api.yaml
  - openapi/facebook-instagram-api.yaml
  - openapi/facebook-marketing-api.yaml
  - openapi/facebook-messenger-api.yaml
  - openapi/facebook-threads-api.yaml
  - openapi/facebook-whatsapp-api.yaml
  type: http
slug: facebook-authentication
source_filename: facebook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/facebook-graph-api.yaml, openapi/facebook-instagram-api.yaml, openapi/facebook-marketing-api.yaml,\n  openapi/facebook-messenger-api.yaml, openapi/facebook-threads-api.yaml, openapi/facebook-whatsapp-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token for Facebook Graph API.\n  sources:\n  - openapi/facebook-graph-api.yaml\n  - openapi/facebook-instagram-api.yaml\n  - openapi/facebook-marketing-api.yaml\n  - openapi/facebook-messenger-api.yaml\n  - openapi/facebook-threads-api.yaml\n  - openapi/facebook-whatsapp-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/authentication/facebook-authentication.yml
summary_line: http · 1 scheme
tags:
- Fortune 500
- Advertising
- Content Publishing
- Messaging
- Social Media
- Social Networking
---
