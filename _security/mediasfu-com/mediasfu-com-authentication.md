---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mediasfu-com-openapi-generated.yml
  format: yaml
  label: MediaSFU API
  slug: mediasfu-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediasfu-com/openapi/_ae-authored/mediasfu-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MediaSFU Authentication
name_suffix: Authentication
oauth_flows: []
overview: MediaSFU declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MediaSFU
provider_slug: mediasfu-com
scheme_count: 1
schemes:
- evidence: 'Where does the key go in a request? Into a single Authorization header, as your username and key joined by a colon: Bearer apiUserName:apiKey.'
  header: Authorization
  how_to_obtain: Create a key in the dashboard and copy the apiUserName and apiKey.
  location: header
  name: Authorization
  type: apiKey
slug: mediasfu-com-authentication
source_filename: mediasfu-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mediasfu.com/api-keys
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mediasfu.com/api-keys\nsources:\n- https://mediasfu.com/api-keys\n- https://mediasfu.com/docs/usage/secure-backend-proxy/\n- https://mediasfu.com/docs/usage/quickstart/\n- https://mediasfu.com/docs/usage/quickstart/\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: 'Where does the key go in a request? Into a single Authorization header, as your username and key joined by a colon: Bearer apiUserName:apiKey.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the dashboard and copy the apiUserName and apiKey.\ndocs: https://mediasfu.com/api-keys\n"
source_yaml_url: https://artifacts.apis.io/mediasfu-com/authentication/mediasfu-com-authentication.yml
summary_line: 1 scheme
tags:
- Video
- Voice
- Artificial Intelligence
- WebRTC
- SDK
- Real-Time Communication
- Live Translation
- Meetings
---
