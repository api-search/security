---
api_key_in:
- header
api_specs:
- filename: angelcam-openapi-original.yml
  format: yaml
  label: Angelcam API
  slug: angelcam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/angelcam/refs/heads/main/openapi/angelcam-openapi-original.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Angelcam Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
overview: AngelCam secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and password flow(s).
provider_name: AngelCam
provider_slug: angelcam
scheme_count: 2
schemes:
- description: See the Authentication section above for full documentation.
  flows:
  - authorizationUrl: https://my.angelcam.com/oauth/authorize/
    flow: authorizationCode
    scopes: 38
    tokenUrl: https://my.angelcam.com/oauth/token/
  - flow: password
    scopes: 40
    tokenUrl: https://api.angelcam.com/oauth/token/
  name: OAuth2
  sources:
  - openapi/angelcam-openapi-original.yml
  type: oauth2
- description: 'Enter your token as: `PersonalAccessToken {your-token}`'
  in: header
  name: PersonalAccessToken
  parameter: Authorization
  sources:
  - openapi/angelcam-openapi-original.yml
  type: apiKey
slug: angelcam-authentication
source_filename: angelcam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/angelcam-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - password\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://my.angelcam.com/oauth/authorize/\n    tokenUrl: https://my.angelcam.com/oauth/token/\n    scopes: 38\n  - flow: password\n    tokenUrl: https://api.angelcam.com/oauth/token/\n    scopes: 40\n  description: See the Authentication section above for full documentation.\n  sources:\n  - openapi/angelcam-openapi-original.yml\n- name: PersonalAccessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Enter your token as: `PersonalAccessToken {your-token}`'\n  sources:\n  - openapi/angelcam-openapi-original.yml\ndocs: https://developers.angelcam.com/guides/authentication/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angelcam/refs/heads/main/authentication/angelcam-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Video Surveillance
- Cameras
- IP Camera
- Cloud Recording
- Video Streaming
- IoT
- ONVIF
- Security
- Webhooks
---
