---
api_key_in: []
auth_types:
- oauth2
- http
description: 'Campaign Monitor publishes no OpenAPI, so this profile was read from the provider''s own Getting Started page rather than derived from securitySchemes. The API supports exactly two authentication models: OAuth 2.0 (preferred for third-party integrations) and an API key over HTTP Basic (username = API key, password ignored).'
kind: authentication
layout: security
method: searched
name: Campaignmonitor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Campaign Monitor secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Campaign Monitor
provider_slug: campaignmonitor
scheme_count: 2
schemes:
- description: OAuth 2.0. Applications are registered inside the Campaign Monitor account (Integrations -> OAuth Registration) and issued a Client ID and Client Secret. Access tokens are passed as bearer tokens.
  discovery_document: false
  errors:
  - code: invalid_request
    meaning: Required parameters were not supplied.
  - code: unknown_client
    meaning: The client_id did not match a registered integration.
  - code: invalid_redirect_uri
    meaning: The redirect_uri did not begin with the registered redirect URI.
  - code: server_error
    meaning: Something went wrong at the Campaign Monitor end.
  - code: unknown_scope
    meaning: Unrecognised permissions were requested via the scope parameter.
  - code: access_denied
    meaning: The end-user did not grant authorisation.
  flows:
  - authorization_url: https://api.createsend.com/oauth
    label: Web Application Flow
    name: authorization_code
    refresh: Long-lived refresh_token returned with the grant; POST grant_type=refresh_token&refresh_token={refresh_token} to https://api.createsend.com/oauth/token
    required_query_params:
      client_id: The Client ID issued at registration
      redirect_uri: Must begin with the redirect URI registered for the application (scheme, authority and path elements must match)
      scope: Comma-separated list of permissions
      state: Optional passthrough state
      type: web_server
    token_url: https://api.createsend.com/oauth/token
  - authorization_url: https://api.createsend.com/oauth
    label: Non-Web Application Flow (desktop / native)
    name: implicit
    refresh: No refresh token is issued in this flow. Clients must use the expires_in value returned in the URL fragment to decide when to request a new token.
    required_query_params:
      client_id: The Client ID issued at registration
      redirect_uri: Must begin with the registered redirect URI
      scope: Comma-separated list of permissions
      type: user_agent
    token_url: null
  name: oauth2
  pkce: false
  scope_delimiter: ','
  scopes_artifact: scopes/campaignmonitor-scopes.yml
  token:
    expires_in_seconds: 1209600
    format: 'Authorization: Bearer {access_token}'
    note: expires_in is returned per grant; the documented example value is 1209600 seconds (14 days).
    transport: Authorization request header
  type: oauth2
- description: API key over HTTP Basic authentication. The API key is supplied as the Basic username; the password portion is unused and may be blank or a dummy value. Keys are retrieved from Account Settings -> API keys in the app.
  key_prefix: null
  key_scope:
  - account-level API key (agency/account wide — client must then be named explicitly on agency endpoints)
  - client-specific API key (implies the client, so clientID parameters can be omitted)
  name: apiKeyBasic
  note: Campaign Monitor does not publish a key prefix convention or a documented rotation/expiry policy for API keys.
  rotation_policy: null
  scheme: basic
  type: http
slug: campaignmonitor-authentication
source_filename: campaignmonitor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.campaignmonitor.com/api/v3-3/getting-started/\ndocs: https://www.campaignmonitor.com/api/v3-3/getting-started/\ndescription: >-\n  Campaign Monitor publishes no OpenAPI, so this profile was read from the\n  provider's own Getting Started page rather than derived from securitySchemes.\n  The API supports exactly two authentication models: OAuth 2.0 (preferred for\n  third-party integrations) and an API key over HTTP Basic (username = API key,\n  password ignored).\nbase_url: https://api.createsend.com/api/v3.3\nsummary:\n  types: [oauth2, http]\n  preferred: oauth2\n  mfa_on_api: false\n  mtls: false\n  openid_connect: false\nschemes:\n  - name: oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.0. Applications are registered inside the Campaign Monitor account\n      (Integrations -> OAuth Registration) and issued a Client ID and Client\n      Secret. Access tokens are passed as bearer tokens.\n    flows:\n\
  \      - name: authorization_code\n        label: Web Application Flow\n        authorization_url: https://api.createsend.com/oauth\n        token_url: https://api.createsend.com/oauth/token\n        required_query_params:\n          type: web_server\n          client_id: The Client ID issued at registration\n          redirect_uri: Must begin with the redirect URI registered for the application (scheme, authority and path elements must match)\n          scope: Comma-separated list of permissions\n          state: Optional passthrough state\n        refresh: >-\n          Long-lived refresh_token returned with the grant; POST\n          grant_type=refresh_token&refresh_token={refresh_token} to\n          https://api.createsend.com/oauth/token\n      - name: implicit\n        label: Non-Web Application Flow (desktop / native)\n        authorization_url: https://api.createsend.com/oauth\n        token_url: null\n        required_query_params:\n          type: user_agent\n          client_id:\
  \ The Client ID issued at registration\n          redirect_uri: Must begin with the registered redirect URI\n          scope: Comma-separated list of permissions\n        refresh: >-\n          No refresh token is issued in this flow. Clients must use the\n          expires_in value returned in the URL fragment to decide when to\n          request a new token.\n    token:\n      transport: Authorization request header\n      format: \"Authorization: Bearer {access_token}\"\n      expires_in_seconds: 1209600\n      note: expires_in is returned per grant; the documented example value is 1209600 seconds (14 days).\n    scopes_artifact: scopes/campaignmonitor-scopes.yml\n    scope_delimiter: \",\"\n    pkce: false\n    discovery_document: false\n    errors:\n      - code: invalid_request\n        meaning: Required parameters were not supplied.\n      - code: unknown_client\n        meaning: The client_id did not match a registered integration.\n      - code: invalid_redirect_uri\n        meaning:\
  \ The redirect_uri did not begin with the registered redirect URI.\n      - code: server_error\n        meaning: Something went wrong at the Campaign Monitor end.\n      - code: unknown_scope\n        meaning: Unrecognised permissions were requested via the scope parameter.\n      - code: access_denied\n        meaning: The end-user did not grant authorisation.\n  - name: apiKeyBasic\n    type: http\n    scheme: basic\n    description: >-\n      API key over HTTP Basic authentication. The API key is supplied as the\n      Basic username; the password portion is unused and may be blank or a dummy\n      value. Keys are retrieved from Account Settings -> API keys in the app.\n    key_scope:\n      - account-level API key (agency/account wide — client must then be named explicitly on agency endpoints)\n      - client-specific API key (implies the client, so clientID parameters can be omitted)\n    rotation_policy: null\n    key_prefix: null\n    note: >-\n      Campaign Monitor does not publish\
  \ a key prefix convention or a documented\n      rotation/expiry policy for API keys.\nauth_errors:\n  - status: 401\n    code: 100\n    message: Invalid API Key\n  - status: 401\n    code: 120\n    message: Invalid OAuth Token\n  - status: 401\n    code: 121\n    message: Expired OAuth Token\n  - status: 401\n    code: 122\n    message: Revoked OAuth Token\n  - status: 401\n    code: 102\n    message: Invalid ClientID — a resource ID that does not belong to the authenticated account also returns 401, not 403/404\n  - status: 403\n    code: 403\n    message: Not allowed for a Non-agency Customer (agency-only resources)\n  - status: 401\n    code: 60\n    message: You do not have the required permission to access this resource (OAuth token missing the needed permission)\ntransport_security:\n  tls_minimum: TLSv1.2\n  note: >-\n    Campaign Monitor deprecated legacy TLS 1.0 and 1.1; TLS 1.2 is the stated\n    minimum supported protocol (https://www.campaignmonitor.com/api/).\n  detail: security/campaignmonitor-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campaignmonitor/refs/heads/main/authentication/campaignmonitor-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Email Marketing
- Campaigns
- Subscribers
- Transactional Email
- Segments
- Newsletters
- Automation
- Marketing Automation
- Webhook
- Email Deliverability
- Marketing
---
