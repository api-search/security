---
api_key_in:
- header
api_specs:
- filename: zoom-phone-api-openapi.json
  format: json
  label: Zoom Phone API
  slug: zoom-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom-phone/refs/heads/main/openapi/zoom-phone-api-openapi.json
- filename: zoom-phone-webhooks-openapi.json
  format: json
  label: Zoom Phone Webhooks
  slug: zoom-phone-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom-phone/refs/heads/main/openapi/zoom-phone-webhooks-openapi.json
- filename: zoom-phone-number-management-openapi.json
  format: json
  label: Zoom Phone Number Management API
  slug: zoom-phone-number-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom-phone/refs/heads/main/openapi/zoom-phone-number-management-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Zoom Phone Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zoom Phone secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zoom Phone
provider_slug: zoom-phone
scheme_count: 2
schemes:
- in: header
  name: openapi_authorization
  parameter: Authorization
  sources:
  - openapi/zoom-phone-api-openapi.json
  - openapi/zoom-phone-number-management-openapi.json
  type: apiKey
- flows:
  - authorizationUrl: /
    flow: authorizationCode
    scopes: 410
  name: openapi_oauth
  sources:
  - openapi/zoom-phone-api-openapi.json
  - openapi/zoom-phone-number-management-openapi.json
  type: oauth2
slug: zoom-phone-authentication
source_filename: zoom-phone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  openapi/zoom-phone-api-openapi.json, openapi/zoom-phone-number-management-openapi.json,\n  https://developers.zoom.us/docs/integrations/oauth/,\n  https://developers.zoom.us/docs/internal-apps/s2s-oauth/,\n  https://developers.zoom.us/docs/api/using-zoom-apis/,\n  https://api.zoom.us/.well-known/oauth-authorization-server\ndocs: https://developers.zoom.us/docs/integrations/oauth/\nsummary_narrative: >-\n  Zoom Phone accepts exactly one credential: an OAuth 2.0 bearer access token in the\n  Authorization header. The apiKey scheme the specs declare (openapi_authorization, header\n  \"Authorization\") is the spec's representation of that bearer header, not a separate API-key\n  model — there are no Zoom Phone API keys. Four app shapes issue tokens: user-managed OAuth\n  (authorization_code), Server-to-Server OAuth (Zoom's own account_credentials grant, the right\n  choice for provisioning and reporting), device authorization\
  \ (device_code), and client\n  credentials. Access tokens are short-lived and refreshed with refresh_token; the token\n  response carries an api_url naming the region that should serve the account. JWT app\n  credentials survive only for the Video/Meeting SDKs, not the Phone REST API.\noauth_metadata:\n  issuer: https://zoom.us\n  authorization_endpoint: https://zoom.us/oauth/authorize\n  token_endpoint: https://zoom.us/oauth/token\n  grant_types_supported: [authorization_code, refresh_token, client_credentials, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  response_types_supported: [code]\n  service_documentation: https://developers.zoom.us/docs/integrations/oauth/\n  source: https://api.zoom.us/.well-known/oauth-authorization-server (RFC 8414, HTTP 200)\n  openid_connect: false\nwebhook_authentication:\n  signature_header: x-zm-signature\n  timestamp_header: x-zm-request-timestamp\n  algorithm: HMAC-SHA256 over \"v0:{timestamp}:{raw\
  \ body}\" with the app secret token\n  validation: endpoint.url_validation challenge/response\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: openapi_authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n  - openapi/zoom-phone-number-management-openapi.json\n- name: openapi_oauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /\n    scopes: 410\n  sources:\n  - openapi/zoom-phone-api-openapi.json\n  - openapi/zoom-phone-number-management-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoom-phone/refs/heads/main/authentication/zoom-phone-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Telecommunications
- United States
- UCaaS
- Cloud PBX
- Voice
- VoIP
- SIP
- Messaging
- SMS
- Phone Numbers
- Number Porting
- BYOC
- Carrier Peering
- Contact Center
- Communications
---
