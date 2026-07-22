---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Newvoicemedia Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: NewVoiceMedia secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: NewVoiceMedia
provider_slug: newvoicemedia
scheme_count: 1
schemes:
- flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  regions_documented:
  - emea
  request_encoding: application/x-www-form-urlencoded
  request_params:
  - grant_type
  - client_id
  - client_secret
  - scope
  sources:
  - https://docs-vcc.atlassian.net/wiki/spaces/VCCA/pages/3568861545/Getting+a+bearer+access+token
  - https://docs-vcc.atlassian.net/wiki/spaces/VCCA/pages/3599269892/Create+bearer+access+token
  token_endpoint: https://{region}.cc.vonage.com/Auth/connect/token
  token_type: Bearer
  type: oauth2
  usage: 'Authorization: Bearer {access_token}'
slug: newvoicemedia-authentication
source_filename: newvoicemedia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs-vcc.atlassian.net/wiki/spaces/VCCA/pages/3567190030/How+to+authenticate+with+a+Vonage+Contact+Center+(VCC)+API\ndocs: https://docs-vcc.atlassian.net/wiki/spaces/VCCA\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_type: Bearer\nnotes: >-\n  Vonage Contact Center (VCC, formerly NewVoiceMedia) APIs authenticate with\n  OAuth 2.0 client-credentials. A tenant obtains API credentials (client id +\n  client secret) from the VCC admin portal, then POSTs them to the regional\n  token endpoint to receive a short-lived Bearer access token, which is sent as\n  an Authorization: Bearer header on every API request. Scope is requested at\n  token time (see scopes/newvoicemedia-scopes.yml).\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_endpoint: https://{region}.cc.vonage.com/Auth/connect/token\n    grant_type: client_credentials\n    request_encoding:\
  \ application/x-www-form-urlencoded\n    request_params: [grant_type, client_id, client_secret, scope]\n    token_type: Bearer\n    usage: 'Authorization: Bearer {access_token}'\n    regions_documented: [emea]\n    sources:\n      - https://docs-vcc.atlassian.net/wiki/spaces/VCCA/pages/3568861545/Getting+a+bearer+access+token\n      - https://docs-vcc.atlassian.net/wiki/spaces/VCCA/pages/3599269892/Create+bearer+access+token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newvoicemedia/refs/heads/main/authentication/newvoicemedia-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Cloud
- Contact Center
- CCaaS
- Communications
- Customer Experience
- Telephony
- Analytics
---
