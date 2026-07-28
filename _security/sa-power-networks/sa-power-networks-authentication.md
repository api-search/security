---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sa Power Networks Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: SA Power Networks secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: SA Power Networks
provider_slug: sa-power-networks
scheme_count: 2
schemes:
- discovery_status: 200
  endpoints:
    authorization: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/authorize
    end_session: https://customer.portal.sapowernetworks.com.au/meterdata/services/auth/idp/oidc/logout
    introspection: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/introspect
    jwks_uri: https://customer.portal.sapowernetworks.com.au/meterdata/id/keys
    registration: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/register
    revocation: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/revoke
    token: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/token
    userinfo: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/userinfo
  evidence:
  - fetched: '2026-07-27'
    file: well-known/sa-power-networks-meterdata-openid-configuration.json
    httpStatus: 200
    url: https://customer.portal.sapowernetworks.com.au/meterdata/.well-known/openid-configuration
  - fetched: '2026-07-27'
    httpStatus: 200
    note: Salesforce platform REST version index, 37 versions v31.0 (Summer '14) through v67.0 (Summer '26), served anonymously. Vendor platform plumbing exposed by the community host — not an SA Power Networks API, not documented by SA Power Networks, and every data path under it requires a session.
    url: https://customer.portal.sapowernetworks.com.au/services/data
  - fetched: '2026-07-27'
    httpStatus: 401
    note: '[{"message":"Authorization required","errorCode":"INVALID_SESSION_ID"}]'
    url: https://customer.portal.sapowernetworks.com.au/services/data/v60.0
  gate: Registration is not self-serve. A third party must obtain the customer's consent, complete the Authorised Representative Registration form (PDF) and be confirmed eligible by SA Power Networks before an account exists to authenticate.
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://customer.portal.sapowernetworks.com.au/meterdata
  name: meterdata-oidc
  openIdConnectUrl: https://customer.portal.sapowernetworks.com.au/meterdata/.well-known/openid-configuration
  platform: Salesforce Experience Cloud
  response_types_supported:
  - code
  - token
  - token id_token
  scopes: scopes/sa-power-networks-scopes.yml
  surface: '"Your Meter Data" portal (Authorised Representative access to a client''s metering data)'
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
- discovery: none
  discovery_note: https://sapndapr.auth.ap-southeast-2.amazoncognito.com/.well-known/openid-configuration returns 404 — Cognito hosted-UI domains do not serve discovery, and the user pool ID needed to reach the real document is not disclosed. Re-verified 2026-07-27.
  evidence:
  - fetched: '2026-07-27'
    httpStatus: 200
    note: page body is a redirect shim to the Cognito hosted UI with response_type=token
    url: https://dapr.sapowernetworks.com.au/
  - fetched: '2026-07-27'
    httpStatus: 400
    note: returns {"error":"invalid_request"} — endpoint live, bearer token required
    url: https://sapndapr.auth.ap-southeast-2.amazoncognito.com/oauth2/userInfo
  flows:
  - authorizationUrl: https://sapndapr.auth.ap-southeast-2.amazoncognito.com/login
    client_id: 4407rsobdsip2kthm31e9l6fd3
    flow: implicit
    redirect_uri: https://dapr.sapowernetworks.com.au/index.php
    scopes:
    - aws.cognito.signin.user.admin
    - email
    - openid
    - profile
  gate: self-serve sign-up through the Cognito hosted UI
  name: dapr-cognito
  platform: AWS Cognito user pool (ap-southeast-2), portal hosted by Rosetta
  surface: DAPR Network Visualisation Portal (map viewer of network capacity and constraints)
  type: oauth2
slug: sa-power-networks-authentication
source_filename: sa-power-networks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  live anonymous probing of SA Power Networks portal hosts on 2026-07-27, plus the\n  OpenID Connect discovery document published by the meter-data community\ndocs: https://www.sapowernetworks.com.au/industry/access-your-clients-meter-data/\nsummary:\n  types: [openIdConnect, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit]\n  applies_to: portal logins only\n  note: >-\n    SA Power Networks operates no API and therefore has no API authentication model.\n    Both auth surfaces below are human browser logins in front of web applications:\n    an AWS Cognito user pool for the DAPR network-visualisation map viewer, and a\n    Salesforce Experience Cloud identity provider for the \"Your Meter Data\" portal\n    used by Authorised Representatives. There is no client-credentials flow, no API\n    key issuance, no documented token acquisition path for a machine consumer, and\n    no published scope model\
  \ of SA Power Networks' own design.\nschemes:\n- name: meterdata-oidc\n  type: openIdConnect\n  surface: '\"Your Meter Data\" portal (Authorised Representative access to a client''s metering data)'\n  platform: Salesforce Experience Cloud\n  openIdConnectUrl: https://customer.portal.sapowernetworks.com.au/meterdata/.well-known/openid-configuration\n  issuer: https://customer.portal.sapowernetworks.com.au/meterdata\n  discovery_status: 200\n  endpoints:\n    authorization: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/authorize\n    token: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/token\n    userinfo: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/userinfo\n    revocation: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/revoke\n    introspection: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/introspect\n    registration: https://customer.portal.sapowernetworks.com.au/meterdata/services/oauth2/register\n\
  \    end_session: https://customer.portal.sapowernetworks.com.au/meterdata/services/auth/idp/oidc/logout\n    jwks_uri: https://customer.portal.sapowernetworks.com.au/meterdata/id/keys\n  response_types_supported: [code, token, token id_token]\n  id_token_signing_alg_values_supported: [RS256]\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic, private_key_jwt]\n  scopes: scopes/sa-power-networks-scopes.yml\n  gate: >-\n    Registration is not self-serve. A third party must obtain the customer's consent,\n    complete the Authorised Representative Registration form (PDF) and be confirmed\n    eligible by SA Power Networks before an account exists to authenticate.\n  evidence:\n  - url: https://customer.portal.sapowernetworks.com.au/meterdata/.well-known/openid-configuration\n    httpStatus: 200\n    fetched: '2026-07-27'\n    file: well-known/sa-power-networks-meterdata-openid-configuration.json\n  - url: https://customer.portal.sapowernetworks.com.au/services/data\n\
  \    httpStatus: 200\n    fetched: '2026-07-27'\n    note: >-\n      Salesforce platform REST version index, 37 versions v31.0 (Summer '14) through\n      v67.0 (Summer '26), served anonymously. Vendor platform plumbing exposed by the\n      community host — not an SA Power Networks API, not documented by SA Power\n      Networks, and every data path under it requires a session.\n  - url: https://customer.portal.sapowernetworks.com.au/services/data/v60.0\n    httpStatus: 401\n    fetched: '2026-07-27'\n    note: '[{\"message\":\"Authorization required\",\"errorCode\":\"INVALID_SESSION_ID\"}]'\n- name: dapr-cognito\n  type: oauth2\n  surface: DAPR Network Visualisation Portal (map viewer of network capacity and constraints)\n  platform: AWS Cognito user pool (ap-southeast-2), portal hosted by Rosetta\n  flows:\n  - flow: implicit\n    authorizationUrl: https://sapndapr.auth.ap-southeast-2.amazoncognito.com/login\n    client_id: 4407rsobdsip2kthm31e9l6fd3\n    redirect_uri: https://dapr.sapowernetworks.com.au/index.php\n\
  \    scopes: [aws.cognito.signin.user.admin, email, openid, profile]\n  discovery: none\n  discovery_note: >-\n    https://sapndapr.auth.ap-southeast-2.amazoncognito.com/.well-known/openid-configuration\n    returns 404 — Cognito hosted-UI domains do not serve discovery, and the user pool\n    ID needed to reach the real document is not disclosed. Re-verified 2026-07-27.\n  gate: self-serve sign-up through the Cognito hosted UI\n  evidence:\n  - url: https://dapr.sapowernetworks.com.au/\n    httpStatus: 200\n    fetched: '2026-07-27'\n    note: page body is a redirect shim to the Cognito hosted UI with response_type=token\n  - url: https://sapndapr.auth.ap-southeast-2.amazoncognito.com/oauth2/userInfo\n    httpStatus: 400\n    fetched: '2026-07-27'\n    note: 'returns {\"error\":\"invalid_request\"} — endpoint live, bearer token required'\nabsent:\n- api_keys\n- client_credentials\n- mutual_tls\n- developer_registration\n- machine_consumer_path\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sa-power-networks/refs/heads/main/authentication/sa-power-networks-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Distribution Network
- Smart Metering
- Solar
- DER
- Open Data
---
