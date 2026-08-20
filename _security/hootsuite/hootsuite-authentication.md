---
api_key_in:
- header
api_specs:
- filename: hootsuite-rest-api-openapi.yml
  format: yaml
  label: Hootsuite REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/openapi/hootsuite-rest-api-openapi.yml
- filename: hootsuite-analytics-api-openapi.yml
  format: yaml
  label: Hootsuite Analytics REST API
  slug: analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/openapi/hootsuite-analytics-api-openapi.yml
- filename: hootsuite-inbox-api-openapi.yml
  format: yaml
  label: Hootsuite Inbox 2.0 API
  slug: inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/openapi/hootsuite-inbox-api-openapi.yml
- filename: hootsuite-amplify-api-openapi.yml
  format: yaml
  label: Hootsuite Amplify REST API
  slug: amplify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/openapi/hootsuite-amplify-api-openapi.yml
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Hootsuite Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- member_app
- organization_app
- clientCredentials
overview: Hootsuite secures its APIs with oauth2, http, and apiKey across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, member_app, organization_app, and clientCredentials flow(s).
provider_name: Hootsuite
provider_slug: hootsuite
scheme_count: 6
schemes:
- flows:
  - authorizationUrl: https://platform.hootsuite.com/oauth2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://platform.hootsuite.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/hootsuite-rest-api-openapi.yml
  - openapi/hootsuite-analytics-api-openapi.yml
  type: oauth2
- name: Basic_Auth
  scheme: basic
  sources:
  - openapi/hootsuite-rest-api-openapi.yml
  - openapi/hootsuite-inbox-api-openapi.yml
  type: http
  used_for: client authentication on POST /oauth2/token
- name: bearer-token
  scheme: bearer
  sources:
  - openapi/hootsuite-inbox-api-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: TO_BE_CONFIGURED_IN_INBOX_2_0
  name: Oauth2ClientCredentials
  sources:
  - openapi/hootsuite-inbox-api-openapi.yml
  type: oauth2
- in: header
  name: SharedSecret
  parameter: X-Hootsuite-Signature
  sources:
  - openapi/hootsuite-inbox-api-openapi.yml
  type: apiKey
  used_for: verifying Inbox 2.0 webhook callbacks
- name: Amplify
  note: The Amplify Swagger declares NO securityDefinitions at all. Its six operations carry no security requirement in the published contract, even though the API is plainly authenticated. An honest gap in Hootsuite's own specification, recorded rather than filled in.
  sources:
  - openapi/hootsuite-amplify-api-openapi.yml
  type: none-declared
slug: hootsuite-authentication
source_filename: hootsuite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://developer.hootsuite.com/docs/api-authentication,\n  https://developer.hootsuite.com/docs/enabling-oauth-20,\n  https://developer.hootsuite.com/docs/set-up-your-oauth-20-app,\n  https://developer.hootsuite.com/docs/rest-api-faq,\n  https://platform.hootsuite.com/.well-known/oauth-authorization-server,\n  openapi/hootsuite-rest-api-openapi.yml, openapi/hootsuite-analytics-api-openapi.yml,\n  openapi/hootsuite-inbox-api-openapi.yml\ndocs: https://developer.hootsuite.com/docs/api-authentication\nsummary:\n  types:\n  - oauth2\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - refreshToken\n  - member_app\n  - organization_app\n  - clientCredentials\n  primary: OAuth 2.0 authorization code with refresh tokens\ndiscovery:\n  authorization_server_metadata: https://platform.hootsuite.com/.well-known/oauth-authorization-server\n  protected_resource_metadata: https://platform.hootsuite.com/.well-known/oauth-protected-resource\n\
  \  local:\n  - well-known/hootsuite-oauth-authorization-server.json\n  - well-known/hootsuite-oauth-protected-resource.json\n  note: >-\n    Both documents are live and returned HTTP 200 on 2026-08-13. This puts Hootsuite ahead of most\n    marketing SaaS: an agent can negotiate the whole OAuth surface without reading the docs.\nendpoints:\n  authorization: https://platform.hootsuite.com/oauth2/auth\n  token: https://platform.hootsuite.com/oauth2/token\n  refresh: https://platform.hootsuite.com/oauth2/token\n  registration: https://platform.hootsuite.com/oauth2/register\n  registration_note: >-\n    Advertised in the RFC 8414 metadata as an RFC 7591 dynamic client registration endpoint, but\n    NOT documented anywhere in the developer documentation, which instead directs developers to\n    register apps by hand at App directory -> Developer apps.\nclient_authentication:\n  method: HTTP Basic (client_id:client_secret)\n  body_credentials_supported: false\n  note: >-\n    Hootsuite states\
  \ explicitly: \"This endpoint requires that you pass in your client credentials\n    using the HTTP Basic authentication scheme... Including your client credentials in the\n    request-body is not supported.\" The RFC 8414 metadata contradicts this slightly by listing\n    client_secret_post and none among token_endpoint_auth_methods_supported.\ntokens:\n  access_token:\n    type: bearer\n    placement: Authorization header\n    ttl_seconds: 3599\n  refresh_token:\n    expiry: none\n    single_use: true\n    note: >-\n      \"Refresh tokens don't have an expiry but can only be used once.\" Each refresh returns a new\n      access token AND a new refresh token; a client that loses the new one is locked out.\n  authorization_code:\n    ttl: 10 minutes\n    single_use: true\n    revocation_trap: >-\n      \"If an authorization code is used a second time, all tokens granted with the first\n      /oauth2/token call will be revoked.\" A naive retry on a code exchange destroys the session.\n\
  pkce:\n  supported: true\n  methods:\n  - S256\n  source: code_challenge_methods_supported in the authorization server metadata\ngrants:\n- id: authorization_code\n  standard: RFC 6749\n  description: Web-server apps acting on behalf of an interactively authorizing user.\n  required_params:\n  - client_id\n  - response_type=code\n  - redirect_uri\n  - scope\n- id: refresh_token\n  standard: RFC 6749\n  description: Exchange a single-use refresh token for a new access token.\n- id: member_app\n  standard: custom\n  description: >-\n    Act on behalf of a MEMBER who has installed the app. Requires grant_type=member_app plus\n    member_id, with Basic client auth. Only usable for members who have installed the app.\n  note: >-\n    This is the grant Hootsuite recommends for single-customer Analytics ETL integrations, because\n    it needs no interactive browser flow.\n- id: organization_app\n  standard: custom\n  description: >-\n    Act on behalf of an ORGANIZATION that has installed the\
  \ app. Requires\n    grant_type=organization_app plus organization_id, with Basic client auth.\n  restriction: >-\n    Organizations used for prescreen components must be on the Enterprise plan, and the\n    organization-app installation must be configured by Hootsuite.\n- id: client_credentials\n  standard: RFC 6749\n  scope: Inbox 2.0 CRM integration only\n  note: >-\n    Declared in openapi/hootsuite-inbox-api-openapi.yml as Oauth2ClientCredentials with tokenUrl\n    literal \"TO_BE_CONFIGURED_IN_INBOX_2_0\" and scope \"some_scope\". That is placeholder text\n    shipped in a production specification, not a usable configuration - the real values are\n    provisioned per customer.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.hootsuite.com/oauth2/auth\n    tokenUrl: https://platform.hootsuite.com/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/hootsuite-rest-api-openapi.yml\n  - openapi/hootsuite-analytics-api-openapi.yml\n\
  - name: Basic_Auth\n  type: http\n  scheme: basic\n  used_for: client authentication on POST /oauth2/token\n  sources:\n  - openapi/hootsuite-rest-api-openapi.yml\n  - openapi/hootsuite-inbox-api-openapi.yml\n- name: bearer-token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/hootsuite-inbox-api-openapi.yml\n- name: Oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: TO_BE_CONFIGURED_IN_INBOX_2_0\n    scopes: 1\n  sources:\n  - openapi/hootsuite-inbox-api-openapi.yml\n- name: SharedSecret\n  type: apiKey\n  in: header\n  parameter: X-Hootsuite-Signature\n  used_for: verifying Inbox 2.0 webhook callbacks\n  sources:\n  - openapi/hootsuite-inbox-api-openapi.yml\n- name: Amplify\n  type: none-declared\n  sources:\n  - openapi/hootsuite-amplify-api-openapi.yml\n  note: >-\n    The Amplify Swagger declares NO securityDefinitions at all. Its six operations carry no\n    security requirement in the published contract, even though the API is\
  \ plainly authenticated.\n    An honest gap in Hootsuite's own specification, recorded rather than filled in.\nredirect_uris:\n  management: App directory -> Developer apps -> [app] -> Security\n  allowed_schemes:\n  - https://\n  - http://localhost\n  multiple: true\n  restriction: >-\n    Apps that are In Review or Launched cannot change redirect URIs self-serve and must contact\n    Hootsuite Developer Support.\nauthorization_beyond_scopes:\n  model: dashboard permissions\n  levels:\n  - organization (Admin or above, plus custom permissions such as Manage Members / Manage Teams)\n  - team (Admin or Member in Team, plus Manage Social Networks in the Team)\n  - social network (Limited / Editor or above, plus Basic Usage / Publish Message / Publish Message\n      with Approval)\n  matrix: https://developer.hootsuite.com/docs/api-permissions-matrix\n  note: >-\n    OAuth scope is NOT the authorization model. Hootsuite only publishes two scopes; the real\n    access decision is the caller's\
  \ dashboard role, which is why 12 of the 97 published error codes\n    are \"Insufficient permissions to ...\" variants. A correctly-scoped agent will still receive 403s\n    it cannot predict from the contract.\nscopes_detail: scopes/hootsuite-scopes.yml\nsso:\n  saml2: true\n  scim2: true\n  note: >-\n    Hootsuite lists SAML 2.0 SSO as a platform feature and ships 11 SCIM 2.0 operations for user and\n    group provisioning under /scim/v2/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/authentication/hootsuite-authentication.yml
summary_line: oauth2/http/apiKey · 6 schemes
tags:
- Social-Media
- Social Media Management
- Marketing
- Content Scheduling
- Analytics
- Engagement
- Social Listening
- Employee Advocacy
- Customer Service
- SCIM
- Authentication
- Webhook
---
