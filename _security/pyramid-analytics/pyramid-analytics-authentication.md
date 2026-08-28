---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Pyramid Analytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pyramid Analytics declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Pyramid Analytics
provider_slug: pyramid-analytics
scheme_count: 0
schemes: []
slug: pyramid-analytics-authentication
source_filename: pyramid-analytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://help.pyramidanalytics.com/Content/Root/developer/reference/APIs/REST%20API/Using%20REST.htm\ndocs:\n- https://help.pyramidanalytics.com/Content/Root/developer/reference/APIs/REST%20API/Authentication%20APIs.htm\n- https://help.pyramidanalytics.com/Content/Root/developer/reference/APIs/REST%20API/Using%20REST.htm\n- https://help.pyramidanalytics.com/Content/Root/AdminClient/security/authentication/Authentication.htm\nnote: >-\n  Derived from the published documentation only — Pyramid publishes no OpenAPI document at a public\n  URL (the Swagger definition is generated inside each customer's own installation), so the scheme\n  below is read from the reference pages and the curl/Java/C#/Python code snippets Pyramid prints\n  on every API 3.0 method page.\nsecurity_schemes:\n- id: paToken\n  type: apiKey\n  in: header\n  name: paToken\n  description: >-\n    API 3.0 carries the security token in an HTTP request header named\
  \ \"paToken\". The token is not\n    a static key: it is minted by one of the /API3/authentication/* methods from a username and\n    password (or an SSO assertion) and returned as a base64 string. Versions 1 and 2 (both\n    deprecated) instead embedded the token in the JSON request payload rather than a header.\n  observed_in: 'curl -X POST -H \"paToken: [[apiKey]]\" \"http://Your.Server.URL/API3/access/getMe\"'\nauthentication_flows:\n- id: api-login\n  name: API Login\n  description: >-\n    An administrative account posts credentials to /API3/authentication/authenticateUser; the\n    response body is the token string, which is then sent as the paToken header on every subsequent\n    call. Pyramid states explicitly: \"All REST API calls are limited to administrative users only.\"\n  methods:\n  - /API3/authentication/authenticateUser\n  - /API3/authentication/authenticateUserWindows\n  - /API3/authentication/authenticateUserSAML\n  - /API3/authentication/authenticateUserOPENID\n- id:\
  \ client-login\n  name: Client Login\n  description: >-\n    The same authentication call, but the resulting token is written into a browser cookie\n    (PyramidAuth) on the Pyramid domain, which skips the interactive login screen.\n- id: client-login-by-admin-token\n  name: Client Login by Admin Token\n  description: >-\n    Two-phase impersonation for when the end user's password is unknown — an admin authenticates\n    first, then /API3/authentication/authenticateUserByToken exchanges the admin token plus the\n    target username for a user token.\n  methods:\n  - /API3/authentication/authenticateUserByToken\n- id: embed-login\n  name: Embed Login\n  description: >-\n    Issues a token designed to operate from a web domain that is NOT the Pyramid domain, for\n    embedding Pyramid content in a third-party application.\n  methods:\n  - /API3/authentication/authenticateUserEmbed\n  - /API3/authentication/authenticateUserEmbedByToken\n  - /API3/authentication/authenticateUserEmbedWindows\n\
  \  - /API3/authentication/authenticateUserEmbedSAML\n  - /API3/authentication/authenticateUserEmbedOPENID\nidentity_providers:\n- SAML 2.0 (generic, plus documented setups for Okta, Google, AWS, Azure AD)\n- OpenID Connect (generic, plus Google OpenID)\n- Windows Authentication / Active Directory\n- LDAP / LDAPS\n- Multi-factor authentication (product setting)\nprovisioning:\n  supported: true\n  mechanism: IDP user search and auto-provisioning (Active Directory, Azure, Google, Ping, Okta)\n  scim: false\n  note: >-\n    Pyramid documents user search and auto-provisioning against the IDP through its own access APIs\n    (searchExternalUsers, searchExternalGroups, createUsersFromSearch, updateUsersFromSearch). No\n    SCIM 2.0 endpoint or urn:ietf:params:scim schema URN appears anywhere in the published\n    documentation set.\n  source: https://help.pyramidanalytics.com/Content/Root/AdminClient/security/authentication/provisioning/User%20Provisioning%20from%20IDPs.htm\noauth2:\n  supported:\
  \ false\n  note: >-\n    There is no OAuth 2.0 authorization-code flow and no scope surface on the Pyramid REST API —\n    authorization is role-based inside the product, not scope-based on the token. scopes/ is\n    therefore deliberately not emitted rather than being filled with an empty artifact.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pyramid-analytics/refs/heads/main/authentication/pyramid-analytics-authentication.yml
summary_line: 0 schemes
tags:
- Analytics
- Business Intelligence
- Decision Intelligence
- Embedded Analytics
- Data Visualization
- Data Preparation
- Enterprise Software
- Reporting
---
