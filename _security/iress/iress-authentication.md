---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Iress Open (Xplan REST API) authentication. The Swagger contract declares HTTP Basic (Xplan credentials) together with two required headers: the integrator API key (x-xplan-app-id) and the target Xplan site (x-forwarded-host). The community docs state OAuth 2.0 Authorisation Code Grant is the preferred mechanism and that Basic is supported but discouraged. Keys are provisioned by Iress through the Iress API Key Portal (gated).'
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Iress Authentication
name_suffix: Authentication
oauth_flows: []
overview: Iress declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Iress
provider_slug: iress
scheme_count: 4
schemes:
- description: Your XPLAN Credentials
  docs_note: HTTP Basic Authentication is also supported but discouraged due to the necessity to store user credentials.
  name: BasicAuth
  scheme: basic
  source: https://api.iressopen.com.au/swagger/3.0/swagger.json
  two_factor: When 2FA is mandatory the OTP is appended to the password, separated by \n\r\t\u0007, i.e. Base64 of USER:PASSWORD\n\r\t\u0007OTP; after the session is established use the XPLANID session cookie instead of the Authorization header.
  two_factor_source: https://github.com/iress/iress-xplan-api-examples/blob/main/2FA_TECHNICAL_DOC.md
  type: http
- description: Your integrator's API Key
  header: x-xplan-app-id
  in: header
  name: APIKey
  source: https://api.iressopen.com.au/swagger/3.0/swagger.json
  type: apiKey
- description: Target Xplan site to authorise against
  header: x-forwarded-host
  in: header
  name: Target Xplan Site
  source: https://api.iressopen.com.au/swagger/3.0/swagger.json
  type: apiKey
- declared_in_contract: false
  description: Iress API Keys use OAuth 2.0 (Authorisation Code Grant) as their preferred authentication mechanism.
  flow: authorizationCode
  name: OAuth 2.0
  refresh: Iress also support a refresh process whereby a new session can be established programmatically
  session: Once initially established an Xplan session can be maintained for a maximum of one hour before the need to re-authenticate.
  source: https://community.iress.com/ic/discussion/102962/authentication-overview
  type: oauth2
slug: iress-authentication
source_filename: iress-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource:\n- https://api.iressopen.com.au/swagger/3.0/swagger.json\n- https://community.iress.com/ic/discussion/102962/authentication-overview\n- https://community.iress.com/ic/discussion/102964/access-and-authorisation-overview\n- https://github.com/iress/iress-xplan-api-examples/blob/main/2FA_TECHNICAL_DOC.md\ndocs: https://community.iress.com/ic/discussion/102962/authentication-overview\ndescription: 'Iress Open (Xplan REST API) authentication. The Swagger contract declares HTTP Basic (Xplan credentials)\n  together with two required headers: the integrator API key (x-xplan-app-id) and the target Xplan site (x-forwarded-host).\n  The community docs state OAuth 2.0 Authorisation Code Grant is the preferred mechanism and that Basic is supported\n  but discouraged. Keys are provisioned by Iress through the Iress API Key Portal (gated).'\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Your XPLAN Credentials\n\
  \  source: https://api.iressopen.com.au/swagger/3.0/swagger.json\n  docs_note: HTTP Basic Authentication is also supported but discouraged due to the necessity to store user credentials.\n  two_factor: When 2FA is mandatory the OTP is appended to the password, separated by \\n\\r\\t\\u0007, i.e. Base64\n    of USER:PASSWORD\\n\\r\\t\\u0007OTP; after the session is established use the XPLANID session cookie instead of\n    the Authorization header.\n  two_factor_source: https://github.com/iress/iress-xplan-api-examples/blob/main/2FA_TECHNICAL_DOC.md\n- name: APIKey\n  type: apiKey\n  in: header\n  header: x-xplan-app-id\n  description: Your integrator's API Key\n  source: https://api.iressopen.com.au/swagger/3.0/swagger.json\n- name: Target Xplan Site\n  type: apiKey\n  in: header\n  header: x-forwarded-host\n  description: Target Xplan site to authorise against\n  source: https://api.iressopen.com.au/swagger/3.0/swagger.json\n- name: OAuth 2.0\n  type: oauth2\n  flow: authorizationCode\n\
  \  description: Iress API Keys use OAuth 2.0 (Authorisation Code Grant) as their preferred authentication mechanism.\n  session: Once initially established an Xplan session can be maintained for a maximum of one hour before the need\n    to re-authenticate.\n  refresh: Iress also support a refresh process whereby a new session can be established programmatically\n  declared_in_contract: false\n  source: https://community.iress.com/ic/discussion/102962/authentication-overview\nauthorization:\n  model: capabilities\n  description: Authorisation is managed primarily by capabilities, with one set attached to an API Key working in\n    conjunction with those allocated to the Xplan User account connecting to the API.\n  source: https://community.iress.com/ic/discussion/102964/access-and-authorisation-overview\nkey_management:\n  portal: Iress API Key Portal (community category iressapiportal; redirects to auth.id.iress.com login)\n  redirect_uris: Iress API keys can be connected to multiple\
  \ Xplan sites but we support a single redirect URI.\n  source: https://community.iress.com/ic/discussion/102962/authentication-overview\nlegacy:\n- api: Iress Web Services V4 (SOAP)\n  description: 'Session-based: IressSessionStart / ServiceSessionStart request with username@company and password\n    or SAML token (per the Method Reference form and sample XML).'\n  source: https://webservices.iress.com.au/v4/Documentation/MethodReference.aspx\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iress/refs/heads/main/authentication/iress-authentication.yml
summary_line: 4 schemes
tags:
- Financial Data
- Market Data
- Trading
- Wealth Management
- Financial Advice
- Mortgages
- Insurance
- FinTech
---
