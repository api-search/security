---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Callminer Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: CallMiner secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: CallMiner
provider_slug: callminer
scheme_count: 3
schemes:
- description: Machine-to-machine flow used by server-side integrations against the Ingestion and Bulk Export APIs. The client_id and client_secret are issued by CallMiner support, not self-service.
  flow: clientCredentials
  name: CallMinerOAuth2ClientCredentials
  sources:
  - https://idp.callminer.net/.well-known/openid-configuration
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  token_url: https://idp.callminer.net/connect/token
  type: oauth2
- authorization_url: https://idp.callminer.net/connect/authorize
  description: Interactive flow used by CallMiner's own first-party surfaces, including the Swagger UI hosted on the API host. Observed on an anonymous GET of /swagger and /bulkexport/swagger, both of which 302 to /connect/authorize.
  flow: authorizationCode
  name: CallMinerOAuth2AuthorizationCode
  pkce:
    code_challenge_methods:
    - S256
    - plain
    supported: true
  sources:
  - https://api.callminer.net/swagger
  - https://api.callminer.net/bulkexport/swagger
  token_url: https://idp.callminer.net/connect/token
  type: oauth2
- id_token_signing_alg_values_supported:
  - RS256
  issuer: https://idp.callminer.net
  jwks_uri: https://idp.callminer.net/.well-known/openid-configuration/jwks
  name: CallMinerOpenIDConnect
  openid_connect_url: https://idp.callminer.net/.well-known/openid-configuration
  sources:
  - https://idp.callminer.net/.well-known/openid-configuration
  subject_types_supported:
  - public
  type: openIdConnect
slug: callminer-authentication
source_filename: callminer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: https://idp.callminer.net/.well-known/openid-configuration\ndocs: https://api.callminer.net/swagger\nnotes: >-\n  Derived from the CallMiner identity provider's live OpenID Connect discovery\n  document plus the OAuth 2.0 authorization requests the CallMiner Swagger UIs\n  emit when an anonymous client requests them. No OpenAPI document is publicly\n  retrievable, so the security schemes below are observed from the running\n  authorization surface rather than parsed from a spec.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  api_key_in: []\n  identity_provider: https://idp.callminer.net\n  regional: true\nschemes:\n- name: CallMinerOAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://idp.callminer.net/connect/token\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  description: >-\n    Machine-to-machine\
  \ flow used by server-side integrations against the\n    Ingestion and Bulk Export APIs. The client_id and client_secret are issued\n    by CallMiner support, not self-service.\n  sources:\n  - https://idp.callminer.net/.well-known/openid-configuration\n- name: CallMinerOAuth2AuthorizationCode\n  type: oauth2\n  flow: authorizationCode\n  authorization_url: https://idp.callminer.net/connect/authorize\n  token_url: https://idp.callminer.net/connect/token\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n    - plain\n  description: >-\n    Interactive flow used by CallMiner's own first-party surfaces, including the\n    Swagger UI hosted on the API host. Observed on an anonymous GET of\n    /swagger and /bulkexport/swagger, both of which 302 to /connect/authorize.\n  sources:\n  - https://api.callminer.net/swagger\n  - https://api.callminer.net/bulkexport/swagger\n- name: CallMinerOpenIDConnect\n  type: openIdConnect\n  openid_connect_url: https://idp.callminer.net/.well-known/openid-configuration\n\
  \  issuer: https://idp.callminer.net\n  jwks_uri: https://idp.callminer.net/.well-known/openid-configuration/jwks\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  sources:\n  - https://idp.callminer.net/.well-known/openid-configuration\nendpoints:\n  authorization: https://idp.callminer.net/connect/authorize\n  token: https://idp.callminer.net/connect/token\n  userinfo: https://idp.callminer.net/connect/userinfo\n  introspection: https://idp.callminer.net/connect/introspect\n  revocation: https://idp.callminer.net/connect/revocation\n  device_authorization: https://idp.callminer.net/connect/deviceauthorization\n  end_session: https://idp.callminer.net/connect/endsession\n  jwks: https://idp.callminer.net/.well-known/openid-configuration/jwks\ngrant_types_supported:\n- authorization_code\n- client_credentials\n- refresh_token\n- implicit\n- password\n- urn:ietf:params:oauth:grant-type:device_code\nregions:\n  note: >-\n    CallMiner runs region-isolated\
  \ API and identity hosts. Each region has its\n    own issuer; the discovery document above is the US issuer.\n  hosts:\n  - region: US\n    api: https://api.callminer.net\n    idp: https://idp.callminer.net\n  - region: US-FISMA\n    api: https://apif.callminer.net\n    idp: https://idpf.callminer.net\n  - region: UK\n    api: https://apiuk.callminer.net\n    idp: https://idpuk.callminer.net\n  - region: AU\n    api: https://apiaus.callminer.net\n    idp: https://idpaus.callminer.net\n  - region: CA\n    api: https://apica.callminer.net\n    idp: https://idpca.callminer.net\n  - region: EU\n    api: https://apiew.callminer.net\n    idp: https://idpew.callminer.net\n  region_source: https://github.com/Matatika/tap-callminer\ncredential_issuance:\n  self_serve: false\n  note: >-\n    Client credentials are issued by CallMiner rather than obtained through a\n    public developer signup. No public developer portal resolves —\n    developer.callminer.com and partner.callminer.com are NXDOMAIN\
  \ as of the\n    probe date.\nx-evidence:\n  fetched: '2026-08-09'\n  evidence:\n  - url: https://idp.callminer.net/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json\n  - url: https://api.callminer.net/swagger\n    http_status: 302\n    note: redirects to https://idp.callminer.net/connect/authorize then /login\n  - url: https://api.callminer.net/bulkexport/swagger\n    http_status: 302\n    note: redirects to https://idp.callminer.net/connect/authorize then /login\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/callminer/refs/heads/main/authentication/callminer-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Company
- Conversation Intelligence
- Speech Analytics
- Contact Center
- Customer Experience
- Artificial Intelligence
- Analytics
- Transcription
- Quality Management
- Compliance
---
