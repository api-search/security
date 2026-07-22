---
api_key_in:
- header
auth_types:
- apiKey
- custom-token
description: ''
kind: authentication
layout: security
method: searched
name: Panaya Authentication
name_suffix: Authentication
oauth_flows: []
overview: Panaya secures its APIs with apiKey and custom-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Panaya
provider_slug: panaya
scheme_count: 2
schemes:
- description: Long-lived API token passed on every request in the X-Auth-Token header as "email:token" (the Panaya login email, a colon, then the generated token). No login/exchange call required; tokens never expire but can be revoked by an administrator.
  in: header
  login_required: false
  name: api-token
  parameter_name: X-Auth-Token
  source: https://success.panaya.com/docs/authenticating-via-api-with-an-api-token
  token_lifetime: non-expiring-revocable
  type: apiKey
  value_format: email:token
- description: 'Two-step scheme: a user-created access token (optional expiry) is POSTed to /api/accesstoken to receive a short-lived response token valid for 1 hour, which is then used on subsequent API calls.'
  http_method: POST
  name: access-token
  request_content_type: application/x-www-form-urlencoded
  request_params:
  - username
  - token
  response_token_lifetime_seconds: 3600
  source: https://success.panaya.com/docs/how-to-authenticate-to-panaya-via-api-with-an-access-token
  token_endpoints:
  - https://my.panaya.com/api/accesstoken
  - https://emea.panaya.com/api/accesstoken
  type: token-exchange
slug: panaya-authentication
source_filename: panaya-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://success.panaya.com/docs/authenticating-via-api-with-an-api-token\ndocs:\n  - https://success.panaya.com/docs/authenticating-via-api-with-an-api-token\n  - https://success.panaya.com/docs/how-to-authenticate-to-panaya-via-api-with-an-access-token\n  - https://success.panaya.com/docs/how-to-create-your-token\nsummary:\n  types: [apiKey, custom-token]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Panaya exposes two documented, proprietary token auth mechanisms. Neither is\n    OAuth 2.0 / OIDC. Credentials are always prefixed with the account email.\nschemes:\n  - name: api-token\n    type: apiKey\n    in: header\n    parameter_name: X-Auth-Token\n    value_format: \"email:token\"\n    login_required: false\n    token_lifetime: non-expiring-revocable\n    description: >-\n      Long-lived API token passed on every request in the X-Auth-Token header as\n      \"email:token\" (the Panaya login email, a colon,\
  \ then the generated token).\n      No login/exchange call required; tokens never expire but can be revoked by\n      an administrator.\n    source: https://success.panaya.com/docs/authenticating-via-api-with-an-api-token\n  - name: access-token\n    type: token-exchange\n    token_endpoints:\n      - https://my.panaya.com/api/accesstoken\n      - https://emea.panaya.com/api/accesstoken\n    http_method: POST\n    request_content_type: application/x-www-form-urlencoded\n    request_params: [username, token]\n    response_token_lifetime_seconds: 3600\n    description: >-\n      Two-step scheme: a user-created access token (optional expiry) is POSTed to\n      /api/accesstoken to receive a short-lived response token valid for 1 hour,\n      which is then used on subsequent API calls.\n    source: https://success.panaya.com/docs/how-to-authenticate-to-panaya-via-api-with-an-access-token\nadmin_controls:\n  - Monitoring and disabling user tokens (administrator):\n      https://success.panaya.com/docs/how-to-monitor-and-disable-user-tokens-as-administrator\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/panaya/refs/heads/main/authentication/panaya-authentication.yml
summary_line: apiKey/custom-token · 2 schemes
tags:
- Company
- Testing
- Test Automation
- Test Management
- Change Management
- Change Impact Analysis
- ERP
- SAP
- Oracle
- Salesforce
- Quality Assurance
- DevOps
---
