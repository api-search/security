---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Welcome To The Jungle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Welcome to the Jungle declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Welcome to the Jungle
provider_slug: welcome-to-the-jungle
scheme_count: 2
schemes:
- description: Preferred transport. The OAuth access token is sent in the Authorization request header.
  format: 'Authorization: Bearer WK_API_KEY'
  id: oauth_bearer_header
  in: header
  parameter: Authorization
  primary: true
  scheme: bearer
  type: http
- caution: credential-in-url
  description: Documented alternative — the same OAuth access token passed as a query-string parameter. Query-string credentials leak into proxy and server logs and into browser history; the header form should be preferred by any integration that can set headers.
  format: ?access_token=WK_API_KEY
  id: oauth_query_token
  in: query
  parameter: access_token
  primary: false
  type: apiKey
slug: welcome-to-the-jungle-authentication
source_filename: welcome-to-the-jungle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://developers.welcomekit.co/authentication\ndocs: https://developers.welcomekit.co/authentication\napi: Welcome to the Jungle Solutions API\nbase_url: https://www.welcomekit.co/api/v1/external\nsummary: 'The Solutions API is protected by OAuth bearer access tokens with a published scope model.\n  Tokens are not self-service: access is requested through the Welcome to the Jungle help form and the\n  vendor grants the scopes matching the stated use case. There is no OpenAPI document, so this profile\n  is read from the published authentication and scopes pages rather than derived from securitySchemes.'\nschemes:\n- id: oauth_bearer_header\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Bearer WK_API_KEY'\n  primary: true\n  description: Preferred transport. The OAuth access token is sent in the Authorization request header.\n- id: oauth_query_token\n  type: apiKey\n  in:\
  \ query\n  parameter: access_token\n  format: '?access_token=WK_API_KEY'\n  primary: false\n  description: 'Documented alternative — the same OAuth access token passed as a query-string parameter.\n    Query-string credentials leak into proxy and server logs and into browser history; the header form\n    should be preferred by any integration that can set headers.'\n  caution: credential-in-url\ntoken_acquisition:\n  self_service: false\n  flow: manual-grant\n  request_url: https://help.welcometothejungle.com/\n  description: 'No developer console issues keys. The docs state you must request an authentication\n    token through the help form and explain your use case; the vendor then opens the appropriate scopes.\n    Several endpoints (GET /jobs/all, GET /organizations, GET /cms/articles/all) additionally require a\n    dedicated partnership agreement before the su_* / cms_* scopes are granted.'\nscopes_artifact: scopes/welcome-to-the-jungle-scopes.yml\noauth_flows_documented: false\n\
  oauth_metadata_endpoints:\n  authorization_server: null\n  protected_resource: null\n  note: 'Probed 2026-09-04 — /.well-known/oauth-authorization-server and /.well-known/openid-configuration\n    return 404 on www.welcomekit.co, api.welcomekit.co and developers.welcomekit.co. The API uses OAuth\n    scope vocabulary and bearer tokens but publishes no RFC 8414 / OIDC discovery document, and no\n    authorization or token endpoint is documented — tokens are issued out of band.'\nfailure_modes:\n- status: 401\n  error: unauthorized\n  meaning: The OAuth access_token is wrong or missing.\n- status: 403\n  error: invalid_scope\n  meaning: The token is valid but its scope set does not authorize this resource.\ntransport_security:\n  tls_required: true\n  observed_tls: TLSv1.3\n  hsts_on_api_host: false\n  note: 'Observed 2026-09-04 on www.welcomekit.co. TLS 1.3 is served but no Strict-Transport-Security\n    header is returned by the API host; see security/welcome-to-the-jungle-domain-security.yml.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/welcome-to-the-jungle/refs/heads/main/authentication/welcome-to-the-jungle-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Human Resources
- Recruiting
- Applicant Tracking
- Jobs
- Employer Branding
- Talent Acquisition
- HR Tech
- France
---
