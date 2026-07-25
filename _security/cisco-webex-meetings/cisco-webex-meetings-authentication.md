---
api_key_in: []
api_specs:
- filename: cisco-webex-meetings-invitees-api-openapi.yml
  format: yaml
  label: Cisco Webex Meetings Invitees API
  slug: cisco-webex-meetings-invitees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex-meetings/refs/heads/main/openapi/cisco-webex-meetings-invitees-api-openapi.yml
- filename: cisco-webex-meetings-meetings-api-openapi.yml
  format: yaml
  label: Cisco Webex Meetings Meetings API
  slug: cisco-webex-meetings-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex-meetings/refs/heads/main/openapi/cisco-webex-meetings-meetings-api-openapi.yml
- filename: cisco-webex-meetings-recordings-api-openapi.yml
  format: yaml
  label: Cisco Webex Meetings Recordings API
  slug: cisco-webex-meetings-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex-meetings/refs/heads/main/openapi/cisco-webex-meetings-recordings-api-openapi.yml
- filename: cisco-webex-meetings-transcripts-api-openapi.yml
  format: yaml
  label: Cisco Webex Meetings Transcripts API
  slug: cisco-webex-meetings-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-webex-meetings/refs/heads/main/openapi/cisco-webex-meetings-transcripts-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cisco Webex Meetings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Webex Meetings secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cisco Webex Meetings
provider_slug: cisco-webex-meetings
scheme_count: 1
schemes:
- bearerFormat: OAuth2-Access-Token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cisco-webex-meetings-openapi.yml
  type: http
slug: cisco-webex-meetings-authentication
source_filename: cisco-webex-meetings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-webex-meetings-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2-Access-Token\n  sources:\n  - openapi/cisco-webex-meetings-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex-meetings/refs/heads/main/authentication/cisco-webex-meetings-authentication.yml
summary_line: http · 1 scheme
tags:
- Collaboration
- Communications
- Enterprise
- Meetings
- Video Conferencing
---
