---
api_key_in: []
auth_types:
- oauth2
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Avamar Authentication
name_suffix: Authentication
oauth_flows:
- password
- clientCredentials
- authorizationCode
- implicit
overview: Avamar secures its APIs with oauth2, http, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password, clientCredentials, authorizationCode, and implicit flow(s).
provider_name: Avamar
provider_slug: avamar
scheme_count: 5
schemes:
- access_token_ttl_seconds: 1800
  client_registration:
    auth: 'Authorization: Basic base64(user:password) — Avamar admin user'
    body_fields:
    - accessTokenValiditySeconds
    - authorizedGrantTypes
    - autoApproveScopes
    - clientId
    - clientName
    - clientSecret
    - redirectUris
    - refreshTokenValiditySeconds
    - scopes
    content_type: application/json
    method: POST
    url: https://<AvamarServer>/api/v1/oauth2/clients
  description: Primary mechanism for third-party clients. An Avamar administrator first registers an OAuth 2.0 client, then the client exchanges the admin credentials for a bearer access token.
  flow: password
  name: oauth2_password
  refresh_token_ttl_seconds: 43200
  source: https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api
  status: current
  token_endpoint:
    auth: 'Authorization: Basic base64(<CLIENT_ID>:<CLIENT_SECRET>)'
    body_params:
    - grant_type
    - scope
    - username
    - password
    content_type: application/x-www-form-urlencoded
    grant_type: password
    method: POST
    url: https://<AvamarServer>/api/oauth/token
  token_format: JWT (RS256)
  token_response_fields:
  - access_token
  - token_type
  - expires_in
  - scope
  - domain
  - authorized_domain
  - user_name
  - role
  - jti
  token_type: bearer
  type: oauth2
  usage: 'Authorization: Bearer <access_token>'
- description: Optional integration in which the Avamar REST API delegates to a customer-operated OAuth 2.0 authorization server. The customer server provides a token issue endpoint and a token validation endpoint; a client ID and secret are provisioned there for both the customer application and for the Avamar REST API itself.
  flow: clientCredentials
  name: oauth2_customer_server
  source: https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api
  status: current
  type: oauth2
- description: OIDC single sign-on for the Avamar Web UI (AUI), validated by Dell against Keycloak realms. An OIDC client is registered through the Avamar REST API Swagger UI.
  grant_types:
  - implicit
  - refresh_token
  - client_credentials
  - authorization_code
  id_token_signed_response_alg: RS256
  login_pattern: https://<Avamar-utility-node>/aui/?iss=https://<Keycloak-server>:<port>/realms/<realm>
  name: openid_connect_sso
  response_types:
  - code
  - code token
  - token
  scope: read openid profile write
  source: https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api
  status: current
  token_endpoint_auth_method: client_secret_basic
  type: openIdConnect
- description: HTTP Basic with Avamar administrator credentials. Used to bootstrap OAuth 2.0 client registration and to obtain the initial admin token; not intended as the steady-state application credential.
  name: basic_admin
  scheme: basic
  source: https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api
  status: current
  type: http
- description: Legacy scheme used by the separately-installed Avamar REST API server (through Avamar 18.x). A POST to /rest-api/login with HTTP Basic returned a custom X-Concerto-Authorization response header carrying a session token that had to be replayed on every subsequent request; POST /rest-api/logout ended the session. This generation listened on port 8543 at https://RESTAPISERVER:8543/rest-api and no longer appears in the 19.x documentation.
  login: POST https://RESTAPISERVER:8543/rest-api/login
  logout: POST https://RESTAPISERVER:8543/rest-api/logout
  name: concerto_session
  scheme: custom
  session_header: X-Concerto-Authorization
  source: https://www.delltechnologies.com/asset/en-us/products/data-protection/technical-support/docu89854.pdf
  status: retired
  type: http
slug: avamar-authentication
source_filename: avamar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api\ndocs: https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api\nnote: >-\n  Avamar has no public multi-tenant API. Every credential and endpoint below is issued and hosted by\n  the customer's own Avamar server (<AvamarServer> = the IP address or FQDN of that appliance). Values\n  are transcribed verbatim from Dell's published documentation; no credentials are included.\nsummary:\n  types:\n  - oauth2\n  - http\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - password\n  - clientCredentials\n  - authorizationCode\n  - implicit\n  bearer_format: JWT\nschemes:\n- name: oauth2_password\n  type: oauth2\n  flow: password\n  status: current\n  description: >-\n    Primary mechanism for third-party clients. An Avamar administrator first registers an OAuth 2.0\n    client,\
  \ then the client exchanges the admin credentials for a bearer access token.\n  client_registration:\n    method: POST\n    url: https://<AvamarServer>/api/v1/oauth2/clients\n    auth: 'Authorization: Basic base64(user:password) — Avamar admin user'\n    content_type: application/json\n    body_fields:\n    - accessTokenValiditySeconds\n    - authorizedGrantTypes\n    - autoApproveScopes\n    - clientId\n    - clientName\n    - clientSecret\n    - redirectUris\n    - refreshTokenValiditySeconds\n    - scopes\n  token_endpoint:\n    method: POST\n    url: https://<AvamarServer>/api/oauth/token\n    auth: 'Authorization: Basic base64(<CLIENT_ID>:<CLIENT_SECRET>)'\n    content_type: application/x-www-form-urlencoded\n    grant_type: password\n    body_params:\n    - grant_type\n    - scope\n    - username\n    - password\n  token_response_fields:\n  - access_token\n  - token_type\n  - expires_in\n  - scope\n  - domain\n  - authorized_domain\n  - user_name\n  - role\n  - jti\n  token_type:\
  \ bearer\n  token_format: JWT (RS256)\n  access_token_ttl_seconds: 1800\n  refresh_token_ttl_seconds: 43200\n  usage: 'Authorization: Bearer <access_token>'\n  source: https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api\n- name: oauth2_customer_server\n  type: oauth2\n  flow: clientCredentials\n  status: current\n  description: >-\n    Optional integration in which the Avamar REST API delegates to a customer-operated OAuth 2.0\n    authorization server. The customer server provides a token issue endpoint and a token validation\n    endpoint; a client ID and secret are provisioned there for both the customer application and for\n    the Avamar REST API itself.\n  source: https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api\n- name: openid_connect_sso\n  type: openIdConnect\n  status: current\n  description: >-\n    OIDC single sign-on for the Avamar Web UI (AUI), validated by Dell\
  \ against Keycloak realms. An OIDC\n    client is registered through the Avamar REST API Swagger UI.\n  id_token_signed_response_alg: RS256\n  token_endpoint_auth_method: client_secret_basic\n  grant_types:\n  - implicit\n  - refresh_token\n  - client_credentials\n  - authorization_code\n  response_types:\n  - code\n  - code token\n  - token\n  scope: read openid profile write\n  login_pattern: https://<Avamar-utility-node>/aui/?iss=https://<Keycloak-server>:<port>/realms/<realm>\n  source: https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api\n- name: basic_admin\n  type: http\n  scheme: basic\n  status: current\n  description: >-\n    HTTP Basic with Avamar administrator credentials. Used to bootstrap OAuth 2.0 client registration\n    and to obtain the initial admin token; not intended as the steady-state application credential.\n  source: https://www.dell.com/support/manuals/en-us/avamar-server/avamar_administration_guide_19.10/avamar-rest-api\n\
  - name: concerto_session\n  type: http\n  scheme: custom\n  status: retired\n  description: >-\n    Legacy scheme used by the separately-installed Avamar REST API server (through Avamar 18.x). A POST\n    to /rest-api/login with HTTP Basic returned a custom X-Concerto-Authorization response header\n    carrying a session token that had to be replayed on every subsequent request; POST /rest-api/logout\n    ended the session. This generation listened on port 8543 at https://RESTAPISERVER:8543/rest-api and\n    no longer appears in the 19.x documentation.\n  login: POST https://RESTAPISERVER:8543/rest-api/login\n  logout: POST https://RESTAPISERVER:8543/rest-api/logout\n  session_header: X-Concerto-Authorization\n  source: https://www.delltechnologies.com/asset/en-us/products/data-protection/technical-support/docu89854.pdf\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avamar/refs/heads/main/authentication/avamar-authentication.yml
summary_line: oauth2/http/openIdConnect · 5 schemes
tags:
- Company
- Backup
- Data Protection
- Deduplication
- Disaster Recovery
- Storage
- Enterprise Software
- Infrastructure
- Dell Technologies
- On-Premise
---
