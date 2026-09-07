---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Derived entirely from Wand''s own anonymous OpenID Connect discovery document — there is no OpenAPI and no public authentication documentation to read. Wand runs Keycloak at auth.wand.ai; the master realm is the only realm that answers. Nothing here is inferred from prose: every value below is a field of the discovery document saved verbatim at well-known/wand-ai-openid-configuration.json.'
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Wand Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wand declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Wand
provider_slug: wand-ai
scheme_count: 3
schemes:
- description: OpenID Connect 1.0 provider for the Wand platform.
  id: wand_openid_connect
  openIdConnectUrl: https://auth.wand.ai/realms/master/.well-known/openid-configuration
  type: openIdConnect
- flows:
  - authorizationUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/auth
    name: authorization_code
    pkce: true
    pkce_methods:
    - S256
    - plain
    tokenUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/token
  - name: client_credentials
    tokenUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/token
  - name: password
    note: Resource-owner password grant is advertised; discouraged by OAuth 2.1.
    tokenUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/token
  - authorizationUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/auth
    name: implicit
    note: Advertised; discouraged by OAuth 2.1.
  - name: refresh_token
    tokenUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/token
  - deviceAuthorizationUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/auth/device
    grant: urn:ietf:params:oauth:grant-type:device_code
    name: device_code
  - backchannelAuthenticationUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/ext/ciba/auth
    grant: urn:openid:params:grant-type:ciba
    name: ciba
  id: wand_oauth2
  type: oauth2
- description: 'Certificate-bound access tokens are supported (tls_client_certificate_bound_access_tokens: true) and tls_client_auth is an accepted token-endpoint auth method. mTLS endpoint aliases are published for token, revocation, introspection, device, registration, userinfo, PAR and CIBA.'
  id: wand_mtls
  type: mutualTLS
slug: wand-ai-authentication
source_filename: wand-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://auth.wand.ai/realms/master/.well-known/openid-configuration\nname: Wand authentication profile\ndescription: >-\n  Derived entirely from Wand's own anonymous OpenID Connect discovery document — there is no OpenAPI\n  and no public authentication documentation to read. Wand runs Keycloak at auth.wand.ai; the master\n  realm is the only realm that answers. Nothing here is inferred from prose: every value below is a\n  field of the discovery document saved verbatim at well-known/wand-ai-openid-configuration.json.\nx-evidence:\n  fetched: '2026-09-04'\n  url: https://auth.wand.ai/realms/master/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json;charset=UTF-8\nprovider: Keycloak\nissuer: https://auth.wand.ai/realms/master\nschemes:\n- id: wand_openid_connect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.wand.ai/realms/master/.well-known/openid-configuration\n  description: OpenID\
  \ Connect 1.0 provider for the Wand platform.\n- id: wand_oauth2\n  type: oauth2\n  flows:\n  - name: authorization_code\n    authorizationUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/auth\n    tokenUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/token\n    pkce: true\n    pkce_methods: [S256, plain]\n  - name: client_credentials\n    tokenUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/token\n  - name: password\n    tokenUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/token\n    note: Resource-owner password grant is advertised; discouraged by OAuth 2.1.\n  - name: implicit\n    authorizationUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/auth\n    note: Advertised; discouraged by OAuth 2.1.\n  - name: refresh_token\n    tokenUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/token\n  - name: device_code\n    deviceAuthorizationUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/auth/device\n\
  \    grant: 'urn:ietf:params:oauth:grant-type:device_code'\n  - name: ciba\n    backchannelAuthenticationUrl: https://auth.wand.ai/realms/master/protocol/openid-connect/ext/ciba/auth\n    grant: 'urn:openid:params:grant-type:ciba'\n- id: wand_mtls\n  type: mutualTLS\n  description: >-\n    Certificate-bound access tokens are supported (tls_client_certificate_bound_access_tokens: true)\n    and tls_client_auth is an accepted token-endpoint auth method. mTLS endpoint aliases are\n    published for token, revocation, introspection, device, registration, userinfo, PAR and CIBA.\nendpoints:\n  authorization: https://auth.wand.ai/realms/master/protocol/openid-connect/auth\n  token: https://auth.wand.ai/realms/master/protocol/openid-connect/token\n  userinfo: https://auth.wand.ai/realms/master/protocol/openid-connect/userinfo\n  introspection: https://auth.wand.ai/realms/master/protocol/openid-connect/token/introspect\n  revocation: https://auth.wand.ai/realms/master/protocol/openid-connect/revoke\n\
  \  end_session: https://auth.wand.ai/realms/master/protocol/openid-connect/logout\n  jwks: https://auth.wand.ai/realms/master/protocol/openid-connect/certs\n  registration: https://auth.wand.ai/realms/master/clients-registrations/openid-connect\n  pushed_authorization_request: https://auth.wand.ai/realms/master/protocol/openid-connect/ext/par/request\n  device_authorization: https://auth.wand.ai/realms/master/protocol/openid-connect/auth/device\n  backchannel_authentication: https://auth.wand.ai/realms/master/protocol/openid-connect/ext/ciba/auth\ntoken_endpoint_auth_methods:\n- private_key_jwt\n- client_secret_basic\n- client_secret_post\n- tls_client_auth\n- client_secret_jwt\nresponse_modes:\n- query\n- fragment\n- form_post\n- query.jwt\n- fragment.jwt\n- form_post.jwt\n- jwt\nclaims:\n- aud\n- sub\n- iss\n- auth_time\n- name\n- given_name\n- family_name\n- preferred_username\n- email\n- acr\nfeatures:\n  pkce: true\n  par_supported: true\n  par_required: false\n  jarm: true\n  request_object:\
  \ true\n  iss_in_authorization_response: true\n  front_channel_logout: true\n  back_channel_logout: true\ngaps:\n- >-\n  No public API-key or bearer-token documentation exists for the Wand AI Workforce API at\n  api.wand.ai. Whether that API accepts these OIDC tokens could not be confirmed — every probed\n  path returned HTTP 503 and Wand publishes no developer reference.\n- >-\n  Only the Keycloak `master` realm answers. If tenants are provisioned in per-customer realms,\n  those realm names are not publicly discoverable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wand-ai/refs/heads/main/authentication/wand-ai-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agentic AI
- Enterprise Software
- Workforce Automation
- Orchestration
- Process Automation
- Collaboration
- Governance
---
