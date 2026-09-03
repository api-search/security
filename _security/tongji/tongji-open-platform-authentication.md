---
api_key_in: []
api_specs:
- filename: tongji-reference-metadata-openapi.yml
  format: yaml
  label: Tongji University Open Platform
  slug: open-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tongji/refs/heads/main/openapi/tongji-reference-metadata-openapi.yml
auth_types:
- none
- oauth2
- openid-connect
- bearer
description: ''
kind: authentication
layout: security
method: probed
name: Tongji Open Platform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tongji University secures its APIs with none, oauth2, openid-connect, and bearer across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tongji University
provider_slug: tongji
scheme_count: 4
schemes:
- applies_to: https://api.tongji.edu.cn/v1/metadata/, https://api.tongji.edu.cn/v2/metadata/
  description: Thirteen reference-metadata interfaces are documented as 无需授权可直接访问 ("directly accessible, no authorization required") and were confirmed callable with no credential on 2026-09-01, each returning HTTP 200 application/json with the standard {code,data,msg} envelope and code A00000. This is the only openly callable public API surface Tongji University operates that this pipeline could confirm.
  evidence:
  - content_type: application/json; charset=utf-8
    detail: Returned four gender code-table rows with no Authorization header.
    status: 200
    url: https://api.tongji.edu.cn/v1/metadata/user/sex_code
  - content_type: application/json; charset=utf-8
    detail: Returned 23 campus and campus-gate reference rows with no Authorization header.
    status: 200
    url: https://api.tongji.edu.cn/v1/metadata/asset/campus_gate
  - content_type: application/json; charset=utf-8
    detail: Returned 100 dormitory-building reference rows with no Authorization header.
    status: 200
    url: https://api.tongji.edu.cn/v2/metadata/student/accom_building_code
  name: AnonymousMetadata
  operator: institution
  type: none
- applies_to: https://api.tongji.edu.cn/v1/, https://api.tongji.edu.cn/v2/
  description: Machine-to-machine interfaces (客户端模式) are called with an access token obtained from the Keycloak realm using client_id and client_secret issued through the platform's application-and-approval process. The platform also documents a legacy token exchange at POST https://api.tongji.edu.cn/v1/token, which answers HTTP 405 to GET, confirming the route is live and method-restricted.
  evidence:
  - status: 200
    url: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/.well-known/openid-configuration
  - detail: Method Not Allowed on GET — the documented POST token route exists.
    status: 405
    url: https://api.tongji.edu.cn/v1/token
  flow: client_credentials
  name: OpenPlatformClientCredentials
  operator: institution
  token_endpoint: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/token
  type: oauth2
- applies_to: Interfaces documented as 授权码模式 (user-context data)
  authorization_endpoint: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/auth
  description: User-context interfaces use the OIDC authorization-code flow against the same realm, with kc_idp_hint=tjiam brokering to the university's own identity-and-access-management identity provider. The platform states the flow is integrated with the university's CAS deployment and interoperates with campus single sign-on, while requiring applications to keep their own session independent of the SSO session.
  end_session_endpoint: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/logout
  flow: authorization_code
  name: OpenPlatformAuthorizationCode
  operator: institution
  pkce_supported:
  - plain
  - S256
  token_endpoint: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/token
  type: openid-connect
  userinfo_endpoint: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/userinfo
- applies_to: Every non-anonymous interface
  description: 'Whatever flow issued it, the access token is presented as `Authorization: Bearer <access_token>`. The platform documents a 7200-second default lifetime, asks callers to cache the token rather than re-request it, and returns 401 when the token is expired or unauthorized and 403 when the token''s scope does not cover the interface.'
  name: BearerToken
  operator: institution
  type: bearer
slug: tongji-open-platform-authentication
source_filename: tongji-open-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live fetch on 2026-09-01 of the Open Platform's own OpenID Connect discovery document\n  https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/.well-known/openid-configuration\n  (HTTP 200, application/json, 19,727 bytes) and of the realm root\n  https://api.tongji.edu.cn/keycloak/realms/OpenPlatform (HTTP 200), read together with the\n  platform's published authentication guide\n  https://api.tongji.edu.cn/docs/intro/develop/authentication (HTTP 200) and scope guide\n  https://api.tongji.edu.cn/docs/intro/develop/scopes (HTTP 200). Anonymous access was\n  confirmed by unauthenticated GETs against thirteen documented interfaces.\nprovider: Tongji University\nproviderId: tongji\nx-operator: institution\noperator_basis: >-\n  Every endpoint below is under api.tongji.edu.cn, the university's own registrable domain,\n  resolving to 202.120.182.237 in CERNET-CN (China Education and Research Network) address\n  space. The\
  \ authorization server is a Keycloak deployment the university runs itself in a\n  realm it named OpenPlatform; it is not a shared vendor tenancy and no vendor host appears\n  anywhere in the flow.\nsummary:\n  types:\n  - none\n  - oauth2\n  - openid-connect\n  - bearer\n  authorization_server: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform\n  software: Keycloak\n  anonymous_interfaces_confirmed: 13\n  access_token_default_lifetime_seconds: 7200\nschemes:\n- name: AnonymousMetadata\n  type: none\n  operator: institution\n  applies_to: https://api.tongji.edu.cn/v1/metadata/, https://api.tongji.edu.cn/v2/metadata/\n  description: >-\n    Thirteen reference-metadata interfaces are documented as 无需授权可直接访问 (\"directly\n    accessible, no authorization required\") and were confirmed callable with no credential on\n    2026-09-01, each returning HTTP 200 application/json with the standard {code,data,msg}\n    envelope and code A00000. This is the only openly callable public API surface\
  \ Tongji\n    University operates that this pipeline could confirm.\n  evidence:\n  - url: https://api.tongji.edu.cn/v1/metadata/user/sex_code\n    status: 200\n    content_type: application/json; charset=utf-8\n    detail: Returned four gender code-table rows with no Authorization header.\n  - url: https://api.tongji.edu.cn/v1/metadata/asset/campus_gate\n    status: 200\n    content_type: application/json; charset=utf-8\n    detail: Returned 23 campus and campus-gate reference rows with no Authorization header.\n  - url: https://api.tongji.edu.cn/v2/metadata/student/accom_building_code\n    status: 200\n    content_type: application/json; charset=utf-8\n    detail: Returned 100 dormitory-building reference rows with no Authorization header.\n- name: OpenPlatformClientCredentials\n  type: oauth2\n  flow: client_credentials\n  operator: institution\n  applies_to: https://api.tongji.edu.cn/v1/, https://api.tongji.edu.cn/v2/\n  description: >-\n    Machine-to-machine interfaces (客户端模式) are\
  \ called with an access token obtained from the\n    Keycloak realm using client_id and client_secret issued through the platform's\n    application-and-approval process. The platform also documents a legacy token exchange at\n    POST https://api.tongji.edu.cn/v1/token, which answers HTTP 405 to GET, confirming the route\n    is live and method-restricted.\n  token_endpoint: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/token\n  evidence:\n  - url: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/.well-known/openid-configuration\n    status: 200\n  - url: https://api.tongji.edu.cn/v1/token\n    status: 405\n    detail: Method Not Allowed on GET — the documented POST token route exists.\n- name: OpenPlatformAuthorizationCode\n  type: openid-connect\n  flow: authorization_code\n  operator: institution\n  applies_to: Interfaces documented as 授权码模式 (user-context data)\n  description: >-\n    User-context interfaces use the OIDC authorization-code flow\
  \ against the same realm, with\n    kc_idp_hint=tjiam brokering to the university's own identity-and-access-management identity\n    provider. The platform states the flow is integrated with the university's CAS deployment\n    and interoperates with campus single sign-on, while requiring applications to keep their own\n    session independent of the SSO session.\n  authorization_endpoint: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/auth\n  token_endpoint: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/token\n  userinfo_endpoint: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/userinfo\n  end_session_endpoint: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/logout\n  pkce_supported:\n  - plain\n  - S256\n- name: BearerToken\n  type: bearer\n  operator: institution\n  applies_to: Every non-anonymous interface\n  description: >-\n    Whatever flow issued it, the\
  \ access token is presented as `Authorization: Bearer\n    <access_token>`. The platform documents a 7200-second default lifetime, asks callers to\n    cache the token rather than re-request it, and returns 401 when the token is expired or\n    unauthorized and 403 when the token's scope does not cover the interface.\ndiscovery:\n  issuer: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform\n  jwks_uri: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/certs\n  introspection_endpoint: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/token/introspect\n  revocation_endpoint: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/revoke\n  registration_endpoint: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/clients-registrations/openid-connect\n  device_authorization_endpoint: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/auth/device\n  pushed_authorization_request_endpoint:\
  \ https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/ext/par/request\n  backchannel_authentication_endpoint: https://api.tongji.edu.cn/keycloak/realms/OpenPlatform/protocol/openid-connect/ext/ciba/auth\n  grant_types_supported:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\n  token_endpoint_auth_methods_supported:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\nnotes: >-\n  The discovery document advertises an open dynamic client registration endpoint path, but\n  registration on a Keycloak realm is normally gated by an initial access token; this pipeline\n  did not attempt a registration and makes no claim that it is open. Access to non-anonymous\n  interfaces is granted per application by the Information Office, not self-service.\nmaintainers:\n- FN: Kin\
  \ Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tongji/refs/heads/main/authentication/tongji-open-platform-authentication.yml
summary_line: none/oauth2/openid-connect/bearer · 4 schemes
tags:
- University
- Higher Education
- Education
- China
- Shanghai
- Double First-Class
- Open Platform
- Campus Data
- Identity Federation
- Research Data
- Library
- Course Catalog
- Reference Data
---
