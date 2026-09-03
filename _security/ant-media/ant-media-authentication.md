---
api_key_in: []
api_specs:
- filename: ant-media-broadcasts-api-openapi.yml
  format: yaml
  label: Ant Media Broadcasts API
  slug: ant-media-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/openapi/ant-media-broadcasts-api-openapi.yml
- filename: ant-media-filters-api-openapi.yml
  format: yaml
  label: Ant Media Filters API
  slug: ant-media-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/openapi/ant-media-filters-api-openapi.yml
- filename: ant-media-push-notification-api-openapi.yml
  format: yaml
  label: Ant Media Push Notification API
  slug: ant-media-push-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/openapi/ant-media-push-notification-api-openapi.yml
- filename: ant-media-version-api-openapi.yml
  format: yaml
  label: Ant Media Version API
  slug: ant-media-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/openapi/ant-media-version-api-openapi.yml
- filename: ant-media-vods-api-openapi.yml
  format: yaml
  label: Ant Media Vods API
  slug: ant-media-vods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/openapi/ant-media-vods-api-openapi.yml
- filename: ant-media-management-api-openapi.yml
  format: yaml
  label: Ant Media Management API
  slug: ant-media-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/openapi/ant-media-management-api-openapi.yml
- filename: ant-media-cluster-api-openapi.yml
  format: yaml
  label: Ant Media Cluster API
  slug: ant-media-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/openapi/ant-media-cluster-api-openapi.yml
auth_types: []
description: 'Ant Media Server is self-hosted, so authentication is configured per instance rather than issued by a vendor-run identity service. There is no API key or OAuth client to register: the operator turns filters on in the web panel or in red5.properties, and callers present a JWT signed with the instance''s own shared secret — or, for the management panel API, a session cookie obtained with an operator''s e-mail and MD5-hashed password.'
kind: authentication
layout: security
method: searched
name: Ant Media Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ant Media declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Ant Media
provider_slug: ant-media
scheme_count: 4
schemes:
- algorithm: HS256 (HMAC-SHA256)
  applies_to:
  - Ant Media Broadcasts API
  - Ant Media Vods API
  - Ant Media Filters API
  - Ant Media Push Notification API
  - Ant Media Version API
  bearerFormat: JWT
  enabled_by: Web panel — JWT REST API Filter setting (disabled by default)
  example: 'curl -X POST -H "accept: application/json" -H "Content-Type: application/json" -H "Authorization: Bearer {JWTToken}" "https://{domain:5443}/{application}/rest/v2/broadcasts/create" -d ''{"name":"streamName"}'''
  expiry: Optional. The docs describe using the standard JWT `exp` claim (a Unix timestamp); the token is rejected once it passes. No default lifetime is imposed by the server.
  header: Authorization
  id: jwt-rest-api-filter
  scheme: bearer
  secret: A shared secret configured by the operator in the web panel under the JWT REST API Filter setting. There is no per-caller credential; every caller signs with the same key.
  source: https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/jwt-rest-api-filter/
  type: http
  value_form: Bearer {JWTToken}
- applies_to:
  - Ant Media Broadcasts API
  - Ant Media Vods API
  - Ant Media Filters API
  - Ant Media Push Notification API
  description: Instead of a local shared secret the instance can validate REST JWTs against an external OAuth server's JSON Web Key Set. Configured per application in /usr/local/antmedia/webapps/{App-Name}/WEB-INF/red5-web.properties with settings.jwtControlEnabled=true and settings.jwksURL=<issuer>. The documented example issuer is an Auth0 tenant, whose keys are read from <issuer>/.well-known/jwks.json.
  id: jwks
  source: https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/jwt-rest-api-filter/
  type: openIdConnect
- applies_to:
  - Ant Media Management API
  - Ant Media Cluster API
  description: The management panel REST API takes its JWT in a ProxyAuthorization header — NOT Authorization, and with no "Bearer " prefix. Enabled by setting server.jwtServerControlEnabled=true and server.jwtServerSecretKey=<32+ char secret> in conf/red5.properties and restarting the server.
  example: 'curl -X GET -H "Content-Type: application/json" -H "ProxyAuthorization:{JWTToken}" "https://example.com:5443/rest/v2/system-resources"'
  header: ProxyAuthorization
  id: management-jwt
  in: header
  source: https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/management-rest-apis/
  type: apiKey
- applies_to:
  - Ant Media Management API
  - Ant Media Cluster API
  cookie: JSESSIONID
  description: 'Alternative to the management JWT. POST /v2/users/authenticate with a JSON body of {"email": "...", "password": "<MD5 hash of the password>"}; the server returns a JSESSIONID cookie that authorises subsequent management calls. The password is sent as an MD5 hex digest, which is a weak digest by modern standards and is transport-security dependent — always call this over HTTPS on port 5443.'
  id: management-session
  operations:
  - authenticateUser
  - deleteSession
  - isAuthenticatedRest
  - isAdmin
  source: https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/management-rest-apis/
  type: session-cookie
slug: ant-media-authentication
source_filename: ant-media-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Ant Media\nproviderId: ant-media\ngenerated: '2026-09-02'\nmethod: searched\ndocs: https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/jwt-rest-api-filter/\nsource: >-\n  https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/jwt-rest-api-filter/,\n  https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/securing-rest-apis/ and\n  https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/management-rest-apis/\n  (fetched 2026-09-02, HTTP 200 each). The published OpenAPI documents declare no\n  securitySchemes at all, so the whole auth model comes from the documentation.\ndescription: >-\n  Ant Media Server is self-hosted, so authentication is configured per instance rather than\n  issued by a vendor-run identity service. There is no API key or OAuth client to register:\n  the operator turns filters on in the web panel or in red5.properties,\
  \ and callers present a\n  JWT signed with the instance's own shared secret — or, for the management panel API, a\n  session cookie obtained with an operator's e-mail and MD5-hashed password.\ndefault_posture:\n  description: >-\n    Out of the box the REST API is protected by an IP filter, not by a token. The JWT REST API\n    filter is DISABLED by default and the IP filter is ENABLED, restricted to 127.0.0.1 plus\n    whatever the operator adds. An instance exposed to the internet with the IP filter widened\n    and JWT still off has an unauthenticated REST API.\n  source: https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/jwt-rest-api-filter/\nschemes:\n  - id: jwt-rest-api-filter\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    applies_to:\n      - Ant Media Broadcasts API\n      - Ant Media Vods API\n      - Ant Media Filters API\n      - Ant Media Push Notification API\n      - Ant Media Version API\n    header: Authorization\n    value_form: 'Bearer\
  \ {JWTToken}'\n    algorithm: HS256 (HMAC-SHA256)\n    secret: >-\n      A shared secret configured by the operator in the web panel under the JWT REST API\n      Filter setting. There is no per-caller credential; every caller signs with the same key.\n    enabled_by: Web panel — JWT REST API Filter setting (disabled by default)\n    example: >-\n      curl -X POST -H \"accept: application/json\" -H \"Content-Type: application/json\"\n      -H \"Authorization: Bearer {JWTToken}\"\n      \"https://{domain:5443}/{application}/rest/v2/broadcasts/create\" -d '{\"name\":\"streamName\"}'\n    expiry: >-\n      Optional. The docs describe using the standard JWT `exp` claim (a Unix timestamp); the\n      token is rejected once it passes. No default lifetime is imposed by the server.\n    source: https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/jwt-rest-api-filter/\n  - id: jwks\n    type: openIdConnect\n    applies_to:\n      - Ant Media Broadcasts API\n      - Ant Media Vods\
  \ API\n      - Ant Media Filters API\n      - Ant Media Push Notification API\n    description: >-\n      Instead of a local shared secret the instance can validate REST JWTs against an external\n      OAuth server's JSON Web Key Set. Configured per application in\n      /usr/local/antmedia/webapps/{App-Name}/WEB-INF/red5-web.properties with\n      settings.jwtControlEnabled=true and settings.jwksURL=<issuer>. The documented example\n      issuer is an Auth0 tenant, whose keys are read from <issuer>/.well-known/jwks.json.\n    source: https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/jwt-rest-api-filter/\n  - id: management-jwt\n    type: apiKey\n    in: header\n    header: ProxyAuthorization\n    applies_to:\n      - Ant Media Management API\n      - Ant Media Cluster API\n    description: >-\n      The management panel REST API takes its JWT in a ProxyAuthorization header — NOT\n      Authorization, and with no \"Bearer \" prefix. Enabled by setting\n      server.jwtServerControlEnabled=true\
  \ and server.jwtServerSecretKey=<32+ char secret> in\n      conf/red5.properties and restarting the server.\n    example: >-\n      curl -X GET -H \"Content-Type: application/json\" -H \"ProxyAuthorization:{JWTToken}\"\n      \"https://example.com:5443/rest/v2/system-resources\"\n    source: https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/management-rest-apis/\n  - id: management-session\n    type: session-cookie\n    cookie: JSESSIONID\n    applies_to:\n      - Ant Media Management API\n      - Ant Media Cluster API\n    description: >-\n      Alternative to the management JWT. POST /v2/users/authenticate with a JSON body of\n      {\"email\": \"...\", \"password\": \"<MD5 hash of the password>\"}; the server returns a\n      JSESSIONID cookie that authorises subsequent management calls. The password is sent as\n      an MD5 hex digest, which is a weak digest by modern standards and is transport-security\n      dependent — always call this over HTTPS on port 5443.\n\
  \    operations:\n      - authenticateUser\n      - deleteSession\n      - isAuthenticatedRest\n      - isAdmin\n    source: https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/management-rest-apis/\nnetwork_controls:\n  - id: rest-ip-filter\n    description: >-\n      Per-application allow-list of IPs and CIDR ranges configured at\n      Dashboard > {Application} > Settings > IP Filter Settings. Enabled by default with\n      127.0.0.1 allowed. Removing 127.0.0.1 blocks requests originating on the server itself.\n    source: https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/securing-rest-apis/\n  - id: web-panel-cidr\n    description: >-\n      server.allowed_dashboard_CIDR in /usr/local/antmedia/conf/red5.properties restricts which\n      CIDR blocks may reach the web panel. Defaults to 0.0.0.0/0 — everything.\n    source: https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/securing-rest-apis/\nstream_authorization:\n  note: >-\n \
  \   Distinct from REST authentication — these secure publish/play of the media streams, not the\n    management API, and are documented under Stream Security.\n  mechanisms:\n    - id: hash-based-token\n      docs: https://docs.antmedia.io/guides/stream-security/hash-based-token/\n    - id: jwt-stream-security-filter\n      docs: https://docs.antmedia.io/guides/stream-security/jwt-stream-security-filter/\n    - id: one-time-token\n      docs: https://docs.antmedia.io/guides/developer-sdk-and-api/rest-api-guide/\n      operations:\n        - getTokenV2\n        - validateTokenV2\n        - listTokensV2\n        - revokeTokensV2\n        - getJwtTokenV2\n    - id: totp-subscriber\n      description: Time-based one-time passwords per subscriber, with a base32 b32Secret.\n      operations:\n        - addSubscriber\n        - getTOTP\n        - blockSubscriber\n        - revokeSubscribers\n    - id: keycloak-integration\n      docs: https://docs.antmedia.io/guides/stream-security/keycloak-integration/\n\
  \    - id: cors-filter\n      docs: https://docs.antmedia.io/guides/stream-security/cors-filter/\nmaintainers:\n  - FN: Kin Lane\n    email: info@apievangelist.com\n    url: https://apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ant-media/refs/heads/main/authentication/ant-media-authentication.yml
summary_line: 4 schemes
tags:
- Broadcasting
- Live Streaming
- Media
- Streaming
- Video
- WebRTC
---
