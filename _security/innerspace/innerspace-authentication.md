---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Innerspace Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: InnerSpace secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: InnerSpace
provider_slug: innerspace
scheme_count: 2
schemes:
- audience: https://global-config.innerspace.io
  flow: clientCredentials
  name: OAuth2ClientCredentials
  request_fields:
  - client_id
  - client_secret
  - audience
  returns: session_id
  sources:
  - docs:authentication-v2
  token_url: https://api.innerspace.io/v2/oauth/token
  type: oauth2
- description: Session token returned by the /v2/oauth/token exchange, sent on all subsequent calls to https://api.innerspace.io/v2/api
  in: header
  name: SessionHeader
  parameter_name: X-Session-Id
  sources:
  - docs:authentication-v2
  type: apiKey
slug: innerspace-authentication
source_filename: innerspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.innerspace.io/authentication-v2\ndocs: https://developers.innerspace.io/authentication-v2\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  session_token: true\n  note: >-\n    OAuth 2.0 client-credentials exchange returns a session_id (not a bearer\n    access_token). The session_id is supplied on every subsequent GraphQL call\n    via the X-Session-Id header. Sessions expire; clients re-authenticate on 401.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.innerspace.io/v2/oauth/token\n  audience: https://global-config.innerspace.io\n  request_fields:\n  - client_id\n  - client_secret\n  - audience\n  returns: session_id\n  sources:\n  - docs:authentication-v2\n- name: SessionHeader\n  type: apiKey\n  in: header\n  parameter_name: X-Session-Id\n  description: Session token returned by the /v2/oauth/token exchange, sent\
  \ on all\n    subsequent calls to https://api.innerspace.io/v2/api\n  sources:\n  - docs:authentication-v2\ncredentials_provisioning: Contact sales@innerspace.io to obtain a ClientID and ClientSecret;\n  API access is limited to customers with an active contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innerspace/refs/heads/main/authentication/innerspace-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Workplace Analytics
- Occupancy
- Space Utilization
- Real Estate
- Wi-Fi Location
- Building Insights
- GraphQL
- Hybrid Workplace
- PropTech
---
