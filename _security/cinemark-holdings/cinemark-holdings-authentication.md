---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cinemark Holdings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cinemark Holdings declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cinemark Holdings
provider_slug: cinemark-holdings
scheme_count: 1
schemes:
- description: 'Application-level authentication. The portal states that a developer registers an application under the portal''s APPs menu to obtain an App-Token, then sends that token in the header of every request. Verbatim (pt-BR): "Esta API usa somente o nivel de autenticacao de aplicacao... Registre seu aplicativo para obter seu App-Token no menu APPs... Informe seu App-Token no header de cada requisicao."'
  id: app_token
  in: header
  name: App-Token
  note: This is the standard Sensedia API Manager app-token scheme, consistent with the Sensedia tenant Cinemark operates at manager-cinemark-prd.sensedia.com. The exact header spelling could not be verified against a live call because no API endpoint is published and the API Browser is gated.
  type: apiKey
  user_level_auth: false
slug: cinemark-holdings-authentication
source_filename: cinemark-holdings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://developers.cinemark.com.br/api-portal/node/4\ndocs: https://developers.cinemark.com.br/api-portal/node/4\nnote: >-\n  There is no OpenAPI, GraphQL SDL or other machine-readable contract anywhere on a\n  Cinemark host, so nothing here is derived from a spec. Everything below is read from the\n  one auth page the Cinemark Brasil developer portal serves without a login.\n\n  READ THIS CAVEAT BEFORE TRUSTING THE VALUES. The portal is a Sensedia API Portal\n  instance that has been branded for Cinemark but largely NOT customised. On the same\n  auth page, immediately below the Portuguese app-token section transcribed here, the\n  template ships an \"OAuth\" block whose Request-Token, Authorize and Access-Token\n  endpoints are Tumblr's (http://www.tumblr.com/oauth/*). Sibling pages are worse: Terms\n  and Conditions (node/3) and FAQ (node/7) are literal Lorem ipsum, \"Exemplos\" (node/6)\n  references a LIPSUM-java-sdk jar,\
  \ and \"Download SDKs\" (node/8) is Evernote's SDK page\n  copy. Only the app-token section is recorded here; the Tumblr OAuth endpoints are\n  recorded as a deviation and are NOT attributed to Cinemark.\nconfidence: medium\nschemes:\n  - id: app_token\n    type: apiKey\n    in: header\n    name: App-Token\n    description: >-\n      Application-level authentication. The portal states that a developer registers an\n      application under the portal's APPs menu to obtain an App-Token, then sends that\n      token in the header of every request. Verbatim (pt-BR): \"Esta API usa somente o\n      nivel de autenticacao de aplicacao... Registre seu aplicativo para obter seu\n      App-Token no menu APPs... Informe seu App-Token no header de cada requisicao.\"\n    user_level_auth: false\n    note: >-\n      This is the standard Sensedia API Manager app-token scheme, consistent with the\n      Sensedia tenant Cinemark operates at manager-cinemark-prd.sensedia.com. The exact\n      header spelling\
  \ could not be verified against a live call because no API endpoint is\n      published and the API Browser is gated.\noauth2: false\nopenid_connect: false\nmutual_tls: false\ncredential_issuance:\n  method: self-service-registration\n  url: https://developers.cinemark.com.br/api-portal/user/register\n  status: 200\n  note: A free developer account can be created; API access beyond that was not tested.\ndeviations:\n  - id: template-oauth-endpoints\n    description: >-\n      The auth page's OAuth section lists Tumblr's OAuth 1.0a endpoints\n      (http://www.tumblr.com/oauth/request_token, /authorize, /access_token) as if they\n      were this API's. These are Sensedia demo-template placeholders left in place. They\n      are NOT Cinemark endpoints and must never be recorded as such.\ngates:\n  - url: https://developers.cinemark.com.br/api-portal/apis\n    status: 403\n    note: >-\n      The portal's API list (\"Acesso negado\") requires an authenticated developer account,\n      so\
  \ the actual security schemes per API could not be read.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cinemark-holdings/refs/heads/main/authentication/cinemark-holdings-authentication.yml
summary_line: 1 scheme
tags:
- Cinema
- Entertainment
- Loyalty
- Movie Theaters
- Ticketing
- Fortune 1000
---
