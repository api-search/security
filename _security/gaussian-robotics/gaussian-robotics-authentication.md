---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Gaussian Robotics Authentication
name_suffix: Authentication
oauth_flows:
- open-access-token
overview: Gaussian Robotics secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the open-access-token flow(s).
provider_name: Gaussian Robotics
provider_slug: gaussian-robotics
scheme_count: 2
schemes:
- description: Gausium Cloud Open API OAuth 2.0 flow. Developers register in the Gausium developer center to obtain a client_id, client_secret and open_access_key, then exchange them for a bearer access token (with refresh_token) at the token endpoint using the custom open-access grant type.
  flows:
  - flow: open-access-token
    grant_type: urn:gaussian:params:oauth:grant-type:open-access-token
    request_content_type: application/json
    request_params:
    - grant_type
    - client_id
    - client_secret
    - open_access_key
    response_fields:
    - token_type
    - access_token
    - expires_in
    - refresh_token
    tokenUrl: https://openapi.gs-robot.com/gas/api/v1alpha1/oauth/token
  name: OAuth2OpenAccess
  type: oauth2
- applied_to: all Gausium Cloud Open API endpoints (openapi.gs-robot.com)
  description: 'All Gausium Cloud Open API requests carry the OAuth access token in an Authorization Bearer header (e.g. Authorization: Bearer {access_token}).'
  name: BearerAuth
  scheme: bearer
  type: http
slug: gaussian-robotics-authentication
source_filename: gaussian-robotics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer-us.gs-robot.com/en_US/Openapi%20Oauth%20Service/Get%20OAuth%20Token\ndocs: https://developer-us.gs-robot.com/en_US/Be%20A%20Developer%20And%20Create%20A%20Key\nsummary:\n  types: [oauth2, http]\n  http_schemes: [bearer]\n  oauth2_flows: [open-access-token]\nschemes:\n- name: OAuth2OpenAccess\n  type: oauth2\n  description: >-\n    Gausium Cloud Open API OAuth 2.0 flow. Developers register in the Gausium\n    developer center to obtain a client_id, client_secret and open_access_key,\n    then exchange them for a bearer access token (with refresh_token) at the\n    token endpoint using the custom open-access grant type.\n  flows:\n  - flow: open-access-token\n    grant_type: urn:gaussian:params:oauth:grant-type:open-access-token\n    tokenUrl: https://openapi.gs-robot.com/gas/api/v1alpha1/oauth/token\n    request_content_type: application/json\n    request_params: [grant_type, client_id, client_secret, open_access_key]\n\
  \    response_fields: [token_type, access_token, expires_in, refresh_token]\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    All Gausium Cloud Open API requests carry the OAuth access token in an\n    Authorization Bearer header (e.g. Authorization: Bearer {access_token}).\n  applied_to: all Gausium Cloud Open API endpoints (openapi.gs-robot.com)\ncredentials:\n  obtained_at: https://service.gs-robot.com/developer\n  fields: [client_id, client_secret, open_access_key]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gaussian-robotics/refs/heads/main/authentication/gaussian-robotics-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Frontier Tech
- Robotics
- Autonomous Robots
- Cleaning Robots
- IoT
- Fleet Management
- Robot Operations
---
