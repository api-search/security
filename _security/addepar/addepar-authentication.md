---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Addepar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Addepar declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Addepar
provider_slug: addepar
scheme_count: 2
schemes:
- description: 'Base64-encode "Key:Secret" and send as Authorization: Basic <encoded>. Credentials respect the tool and data permissions of the user who created the key. Requires the API Access permission granted by a firm administrator.'
  headers:
  - name: Authorization
    required: true
    value: Basic <base64(Key:Secret)>
  - description: Identifies the firm/organization for the request.
    name: Addepar-Firm
    required: true
    value: <Firm ID>
  - description: Required on POST/PATCH requests (JSON:API media type).
    name: Content-Type
    required: false
    value: application/vnd.api+json
  id: basic
  scheme: basic
  type: http
- authorization_url: provided per-integration by Addepar contact
  description: OAuth 2.0 authorization-code grant for third-party apps accessing user data with limited, granted scopes. Addepar issues client_id, client_secret, and approved scopes; the app supplies redirect URIs and ToS/privacy URLs.
  flow: authorizationCode
  id: oauth2
  scopes_ref: ../scopes/addepar-scopes.yml
  supports_refresh_token: true
  token_url: https://api.addepar.com/public/oauth2/token
  token_url_dev: https://examplefirm.clientdev.addepar.com/api/public/oauth2/token
  type: oauth2
slug: addepar-authentication
source_filename: addepar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developers.addepar.com/docs/basic-authentication + https://developers.addepar.com/docs/oauth\naid: addepar\nname: Addepar API Authentication\ndocs: https://developers.addepar.com/docs/basic-authentication\nsummary: >-\n  The Addepar API supports two authentication mechanisms over HTTPS: HTTP Basic\n  authentication using an API key/secret pair scoped to the creating user's\n  permissions plus an Addepar-Firm header, and OAuth 2.0 authorization-code flow\n  for third-party integrations acting on behalf of a user.\nschemes:\n- id: basic\n  type: http\n  scheme: basic\n  description: >-\n    Base64-encode \"Key:Secret\" and send as Authorization: Basic <encoded>.\n    Credentials respect the tool and data permissions of the user who created\n    the key. Requires the API Access permission granted by a firm administrator.\n  headers:\n  - name: Authorization\n    value: 'Basic <base64(Key:Secret)>'\n    required: true\n\
  \  - name: Addepar-Firm\n    value: '<Firm ID>'\n    required: true\n    description: Identifies the firm/organization for the request.\n  - name: Content-Type\n    value: application/vnd.api+json\n    required: false\n    description: Required on POST/PATCH requests (JSON:API media type).\n- id: oauth2\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    OAuth 2.0 authorization-code grant for third-party apps accessing user data\n    with limited, granted scopes. Addepar issues client_id, client_secret, and\n    approved scopes; the app supplies redirect URIs and ToS/privacy URLs.\n  token_url: https://api.addepar.com/public/oauth2/token\n  token_url_dev: https://examplefirm.clientdev.addepar.com/api/public/oauth2/token\n  authorization_url: provided per-integration by Addepar contact\n  supports_refresh_token: true\n  scopes_ref: ../scopes/addepar-scopes.yml\nnotes:\n- No downloadable OpenAPI found (ReadMe-hosted docs + llms.txt index); profile derived from official docs\
  \ prose.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/addepar/refs/heads/main/authentication/addepar-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Fintech
- Wealth Management
- Portfolio Management
- Investment Management
- Financial Data
- JSON:API
- REST
---
