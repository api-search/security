---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: 1Mind Authentication
name_suffix: Authentication
oauth_flows: []
overview: 1mind declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: 1mind
provider_slug: 1mind
scheme_count: 0
schemes: []
slug: 1mind-authentication
source_filename: 1mind-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://auth.1mind.com/.well-known/openid-configuration (HTTP 200) +\n  https://auth.1mind.com/.well-known/oauth-authorization-server (HTTP 200) +\n  observed WWW-Authenticate challenge on https://auth.1mind.com/userinfo (HTTP 401)\nname: 1mind Authentication\nsummary: >-\n  1mind runs a full OAuth 2.0 / OpenID Connect authorization server at\n  https://auth.1mind.com. It is an Ory-hosted deployment (the host resolves to\n  distracted-wright-ks3ftfdysg.projects.oryapis.com, and Ory is named as the\n  identity-provider subprocessor on 1mind's own sub-processor page), operated\n  under 1mind's own domain and its own issuer identifier. The discovery document\n  is anonymous and machine-readable; the resource APIs it protects are not\n  publicly documented, so the operations a token grants are not enumerable from\n  public sources.\nissuer: https://auth.1mind.com\ndiscovery:\n  openid_configuration: https://auth.1mind.com/.well-known/openid-configuration\n\
  \  oauth_authorization_server: https://auth.1mind.com/.well-known/oauth-authorization-server\n  note: Both endpoints return the same document (1987 bytes, identical).\nsecurity_schemes:\n- key: oauth2\n  type: oauth2\n  description: OAuth 2.0 authorization server with PKCE, refresh tokens and the\n    device authorization grant.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://auth.1mind.com/oauth2/auth\n      tokenUrl: https://auth.1mind.com/oauth2/token\n      refreshUrl: https://auth.1mind.com/oauth2/token\n      pkce: true\n      code_challenge_methods:\n      - S256\n      - plain\n    clientCredentials:\n      tokenUrl: https://auth.1mind.com/oauth2/token\n    deviceCode:\n      deviceAuthorizationUrl: https://auth.1mind.com/oauth2/device/auth\n      tokenUrl: https://auth.1mind.com/oauth2/token\n    implicit:\n      authorizationUrl: https://auth.1mind.com/oauth2/auth\n      note: Advertised in response_types_supported; legacy, not recommended.\n- key: openIdConnect\n\
  \  type: openIdConnect\n  openIdConnectUrl: https://auth.1mind.com/.well-known/openid-configuration\n  description: OpenID Connect 1.0 with RS256-signed ID tokens.\n- key: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Protected endpoints answer HTTP 401 with an RFC 6750 challenge, observed\n    verbatim on https://auth.1mind.com/userinfo:\n    WWW-Authenticate: Bearer error=\"request_unauthorized\",\n    error_description=\"The request could not be authorized. Check that you\n    provided valid credentials in the right format.\"\nendpoints:\n  authorization: https://auth.1mind.com/oauth2/auth\n  token: https://auth.1mind.com/oauth2/token\n  device_authorization: https://auth.1mind.com/oauth2/device/auth\n  revocation: https://auth.1mind.com/oauth2/revoke\n  userinfo: https://auth.1mind.com/userinfo\n  jwks: https://auth.1mind.com/.well-known/jwks.json\n  end_session: https://auth.1mind.com/oauth2/sessions/logout\n  credentials_draft_00: https://auth.1mind.com/credentials\n\
  grant_types_supported:\n- authorization_code\n- implicit\n- client_credentials\n- refresh_token\n- urn:ietf:params:oauth:grant-type:device_code\nresponse_types_supported:\n- code\n- code id_token\n- id_token\n- token id_token\n- token\n- token id_token code\nresponse_modes_supported:\n- query\n- fragment\n- form_post\ntoken_endpoint_auth_methods_supported:\n- client_secret_post\n- client_secret_basic\n- private_key_jwt\n- none\nsigning:\n  id_token_signing_alg_values_supported:\n  - RS256\n  userinfo_signing_alg_values_supported:\n  - none\n  - RS256\n  request_object_signing_alg_values_supported:\n  - none\n  - RS256\n  - ES256\nscopes_supported:\n- openid\n- offline\n- offline_access\nscopes_reference: ../scopes/1mind-scopes.yml\nfeatures:\n  pkce: true\n  refresh_tokens: true\n  device_flow: true\n  private_key_jwt: true\n  request_object: true\n  request_uri: true\n  require_request_uri_registration: true\n  claims_parameter_supported: false\n  backchannel_logout: true\n  frontchannel_logout:\
  \ true\n  verifiable_credentials_draft: true\nclaims_supported:\n- sub\napi_key_auth:\n  documented: false\n  note: >-\n    1mind's public status page lists a component \"US Region - REST API\"\n    described as \"Public 1mind API\", but no public API reference, key-issuance\n    page or authentication guide could be located (see x-coverage in apis.yml).\n    Whether that API accepts OAuth 2.0 bearer tokens from this authorization\n    server, a separate API key, or both, is not stated anywhere public.\ndocs: null\ndocs_note: >-\n  No public authentication documentation exists. developer.1mind.com and\n  docs.1mind.com are NOT developer portals — they are the *.1mind.com wildcard\n  SPA (see well-known/1mind-well-known.yml). The 1mindai/docs GitHub repository\n  is an unmodified Mintlify starter kit.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1mind/refs/heads/main/authentication/1mind-authentication.yml
summary_line: 0 schemes
tags:
- Company
- AI
- AI Agents
- Sales
- Go-To-Market
- Conversational AI
- Sales Enablement
- RevOps
---
