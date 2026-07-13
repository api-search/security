---
api_key_in: []
api_specs:
- filename: mux-openapi.yml
  format: yaml
  label: Mux Video API
  slug: video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mux-com/refs/heads/main/openapi/mux-openapi.yml
- filename: mux-openapi.yml
  format: yaml
  label: Mux Live Streaming API
  slug: live-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mux-com/refs/heads/main/openapi/mux-openapi.yml
- filename: mux-openapi.yml
  format: yaml
  label: Mux Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mux-com/refs/heads/main/openapi/mux-openapi.yml
- filename: mux-openapi.yml
  format: yaml
  label: Mux Stream Delivery API
  slug: stream-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mux-com/refs/heads/main/openapi/mux-openapi.yml
- filename: mux-openapi.yml
  format: yaml
  label: Mux Image API
  slug: image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mux-com/refs/heads/main/openapi/mux-openapi.yml
- filename: mux-openapi.yml
  format: yaml
  label: Mux Robots AI API
  slug: robots-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mux-com/refs/heads/main/openapi/mux-openapi.yml
- filename: mux-openapi.yml
  format: yaml
  label: Mux System API
  slug: system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mux-com/refs/heads/main/openapi/mux-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mux Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mux secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mux
provider_slug: mux-com
scheme_count: 2
schemes:
- description: 'The Mux Video API uses an Access Token and Secret Key for authentication. If you haven''t already, [generate a new Access Token](https://dashboard.mux.com/settings/access-tokens) in the Access Token settings of your Mux account dashboard.


    Once you have an Access Token ID and Secret, you can then simply include those as the username (id) and password (secret) in the same way you use traditional bas'
  name: accessToken
  scheme: basic
  sources:
  - openapi/mux-openapi.yml
  type: http
- description: OAuth authorization token, used as a Bearer Auth header
  name: authorizationToken
  scheme: bearer
  sources:
  - openapi/mux-openapi.yml
  type: http
slug: mux-com-authentication
source_filename: mux-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mux-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessToken\n  type: http\n  scheme: basic\n  description: |-\n    The Mux Video API uses an Access Token and Secret Key for authentication. If you haven't already, [generate a new Access Token](https://dashboard.mux.com/settings/access-tokens) in the Access Token settings of your Mux account dashboard.\n\n    Once you have an Access Token ID and Secret, you can then simply include those as the username (id) and password (secret) in the same way you use traditional bas\n  sources:\n  - openapi/mux-openapi.yml\n- name: authorizationToken\n  type: http\n  scheme: bearer\n  description: OAuth authorization token, used as a Bearer Auth header\n  sources:\n  - openapi/mux-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mux-com/refs/heads/main/authentication/mux-com-authentication.yml
summary_line: http · 2 schemes
tags:
- Video Infrastructure
- Video Streaming
- Live Streaming
- Video Analytics
- Video AI
- Encoding
---
