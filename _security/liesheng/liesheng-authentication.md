---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Liesheng Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Liesheng Group secures its APIs with oauth2, apiKey, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Liesheng Group
provider_slug: liesheng
scheme_count: 3
schemes:
- flows:
  - authorizationUrl: https://cloudapi-oauth.suunto.com/oauth/authorize
    flow: authorizationCode
    scopes:
    - workout
    tokenUrl: https://cloudapi-oauth.suunto.com/oauth/token
  name: SuuntoOAuth2
  refresh_token: true
  request_header: 'Authorization: Bearer <jwt token>'
  source: https://apizone.suunto.com/how-to-start
  token_endpoint_auth: 'HTTP Basic — Authorization: Basic Base64(client_id:client_secret)'
  token_format: JWT
  token_lifetime_seconds: 86400
  type: oauth2
  user_claim: The JWT carries a custom claim `user` holding the authorizing Suunto App account username; used to correlate webhook notifications to a stored token.
- in: header
  keys: primary and secondary, rotatable from the API Zone profile page
  name: Ocp-Apim-Subscription-Key
  required_for: https://cloudapi.suunto.com/ (not required for OAuth endpoints)
  source: https://apizone.suunto.com/how-to-start
  type: apiKey
- applies_to: https://cloudapi-oauth.suunto.com/oauth/token
  name: ClientCredentialsBasic
  scheme: basic
  source: https://apizone.suunto.com/faq
  type: http
slug: liesheng-authentication
source_filename: liesheng-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://apizone.suunto.com/how-to-start\ndocs: https://apizone.suunto.com/how-to-start\nnotes: >-\n  Liesheng Group publishes no API of its own. Its owned brand SUUNTO operates the\n  Suunto Cloud API (Integration API) behind the Suunto API Zone, an Azure API\n  Management developer portal. Access requires acceptance into the Suunto partner\n  program. Every Cloud API call carries TWO credentials: an OAuth2 bearer JWT and\n  an APIM subscription key.\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: SuuntoOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cloudapi-oauth.suunto.com/oauth/authorize\n    tokenUrl: https://cloudapi-oauth.suunto.com/oauth/token\n    scopes:\n    - workout\n  token_format: JWT\n  token_lifetime_seconds: 86400\n  refresh_token: true\n  token_endpoint_auth: >-\n    HTTP\
  \ Basic — Authorization: Basic Base64(client_id:client_secret)\n  request_header: 'Authorization: Bearer <jwt token>'\n  user_claim: >-\n    The JWT carries a custom claim `user` holding the authorizing Suunto App\n    account username; used to correlate webhook notifications to a stored token.\n  source: https://apizone.suunto.com/how-to-start\n- name: ApimSubscriptionKey\n  type: apiKey\n  in: header\n  name: Ocp-Apim-Subscription-Key\n  required_for: https://cloudapi.suunto.com/ (not required for OAuth endpoints)\n  keys: primary and secondary, rotatable from the API Zone profile page\n  source: https://apizone.suunto.com/how-to-start\n- name: ClientCredentialsBasic\n  type: http\n  scheme: basic\n  applies_to: https://cloudapi-oauth.suunto.com/oauth/token\n  source: https://apizone.suunto.com/faq\nonboarding:\n  gated: true\n  process:\n  - Apply to the Suunto partner program at https://www.suunto.com/welcomepartners\n  - Sign the API agreement and name the developers who need API\
  \ Zone access\n  - Subscribe to the Developer API in the API Zone to obtain subscription keys\n  - Configure app name, client secret and redirect URI in the API Zone profile\n  response_time: within two weeks of partner-program acceptance\n  contact: partners@suunto.com\n  personal_use: not offered — companies and organizations only\n  cost: no charge for API use\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liesheng/refs/heads/main/authentication/liesheng-authentication.yml
summary_line: oauth2/apiKey/http · 3 schemes
tags:
- Company
- Consumer Electronics
- Wearables
- Audio
- Sports
- Fitness
- Health
- Internet of Things
- ODM
- OEM
- China
---
