---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Reliance Worldwide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reliance Worldwide declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Reliance Worldwide
provider_slug: reliance-worldwide
scheme_count: 2
schemes:
- description: Sign In into your StreamLabs account at https://my.streamlabswater.com/ and copy your apiKey. You will need an active StreamPlus subscription with API support in order to view your apiKey and use the API. Add the apiKey to your Authorization header of type Bearer.
  header: Authorization
  in: header
  name: apiKey
  scheme: bearer
  source: https://web.archive.org/web/20220930144140/https://developer.streamlabswater.com/docs/getting-started.html
  type: http
- access_token_lifetime_example: 3600 seconds (expires_in in the documented sample response)
  client_registration: To receive OAuth2 credentials, send an email to support@streamlabswater.com with a subject of OAuth 2 Client Request
  description: Used when a company links a user in its system to a StreamLabs customer (example given is Amazon Alexa account linking). Bearer access_token is then sent in the Authorization header.
  flows:
    authorizationCode:
      authorizationUrl: https://auth.streamlabswater.com/login
      refreshUrl: https://auth.streamlabswater.com/oauth2/token
      tokenUrl: https://auth.streamlabswater.com/oauth2/token
  name: oauth2
  redirect_uri_rule: redirect uri and signout uri must begin with https; native apps may register a custom URL scheme
  source: https://web.archive.org/web/20210619122145/https://developer.streamlabswater.com/docs/oauth.html
  token_endpoint_auth: client_secret_basic (Basic Base64Encode(client_id:client_secret))
  type: oauth2
slug: reliance-worldwide-authentication
source_filename: reliance-worldwide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: searched\nsource: https://web.archive.org/web/20210619122145/https://developer.streamlabswater.com/docs/oauth.html\ndocs: https://web.archive.org/web/20220930144140/https://developer.streamlabswater.com/docs/getting-started.html\nnote: Streamlabs Water Developer API (an RWC brand). The developer reference host developer.streamlabswater.com no longer resolves (2026-10-22); these facts are read from Internet Archive captures (2021-06-19 and 2022-09-30). No OpenAPI exists, so nothing is derived.\napi: Streamlabs Water Developer API\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: \"Sign In into your StreamLabs account at https://my.streamlabswater.com/ and copy your apiKey. You will need an active StreamPlus subscription with API support in order to view your apiKey and use the API. Add the apiKey to your Authorization header of type Bearer.\"\n  source: https://web.archive.org/web/20220930144140/https://developer.streamlabswater.com/docs/getting-started.html\n\
  - name: oauth2\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://auth.streamlabswater.com/login\n      tokenUrl: https://auth.streamlabswater.com/oauth2/token\n      refreshUrl: https://auth.streamlabswater.com/oauth2/token\n  token_endpoint_auth: client_secret_basic (Basic Base64Encode(client_id:client_secret))\n  access_token_lifetime_example: 3600 seconds (expires_in in the documented sample response)\n  client_registration: \"To receive OAuth2 credentials, send an email to support@streamlabswater.com with a subject of OAuth 2 Client Request\"\n  redirect_uri_rule: redirect uri and signout uri must begin with https; native apps may register a custom URL scheme\n  description: Used when a company links a user in its system to a StreamLabs customer (example given is Amazon Alexa account linking). Bearer access_token is then sent in the Authorization header.\n  source: https://web.archive.org/web/20210619122145/https://developer.streamlabswater.com/docs/oauth.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reliance-worldwide/refs/heads/main/authentication/reliance-worldwide-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Plumbing
- Manufacturing
- Building Products
- Water Control
- Heating
- ASX Listed
- Australia
---
