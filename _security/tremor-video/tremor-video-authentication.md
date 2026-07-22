---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tremor Video Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Tremor Video secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Tremor Video
provider_slug: tremor-video
scheme_count: 1
schemes:
- applied_as: 'Authorization: Bearer <access_token>'
  credentials:
  - client_id
  - client_secret
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  request_body: JSON body {client_id, client_secret, grant_type=client_credentials}
  sources:
  - https://www.postman.com/nexxen-api/nexxen/documentation/9md8q3a/nexxen-dsp-apis
  tokenUrl: https://services.amobee.com/accounts/v1/api/token
  token_type: Bearer
  type: oauth2
slug: tremor-video-authentication
source_filename: tremor-video-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.postman.com/nexxen-api/nexxen/documentation/9md8q3a/nexxen-dsp-apis\ndocs: https://www.postman.com/nexxen-api/nexxen/documentation/9md8q3a/nexxen-dsp-apis\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_type: Bearer\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  grant_type: client_credentials\n  tokenUrl: https://services.amobee.com/accounts/v1/api/token\n  credentials: [client_id, client_secret]\n  request_body: JSON body {client_id, client_secret, grant_type=client_credentials}\n  token_type: Bearer\n  applied_as: 'Authorization: Bearer <access_token>'\n  sources:\n  - https://www.postman.com/nexxen-api/nexxen/documentation/9md8q3a/nexxen-dsp-apis\nnotes: >-\n  The Nexxen DSP (formerly Amobee / Tremor Video DSP) API uses OAuth2 client-credentials. A client\n  POSTs its client_id and client_secret to the token endpoint and receives an access_token,\
  \ which\n  is then sent as an Authorization: Bearer header on subsequent API calls against\n  https://services.amobee.com/campaign/v3/api. API credentials are generated inside the Nexxen /\n  Amobee DSP platform; the token and call flow are documented in the public Nexxen DSP Postman\n  workspace and corroborated by third-party connectors (Supermetrics) and a community Python\n  client.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/authentication/tremor-video-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Martech
- Advertising
- AdTech
- DSP
- Programmatic
- CTV
- Video Advertising
---
