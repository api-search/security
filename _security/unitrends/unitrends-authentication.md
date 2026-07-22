---
api_key_in: []
api_specs:
- filename: unitrends-public-api-openapi.json
  format: json
  label: Unitrends MSP Public API (UniView Portal)
  slug: unitrends-msp-public-api-uniview-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/openapi/unitrends-public-api-openapi.json
auth_types:
- oauth2
- http-bearer
- session-token
description: ''
kind: authentication
layout: security
method: searched
name: Unitrends Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Unitrends secures its APIs with oauth2, http-bearer, and session-token across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Unitrends
provider_slug: unitrends
scheme_count: 3
schemes:
- description: 'JWT Authorization header using the Bearer scheme. Example value: "Bearer {token}"'
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/unitrends-public-api-openapi.json
  type: apiKey
- api: Unitrends MSP Public API (UniView Portal)
  client_auth_methods:
  - client_secret_post
  - private_key_jwt
  - client_secret_basic
  credential_issuance: 'Create public API credentials in the UniView Portal (API Access view > + New); the portal issues a Client ID and Client Secret (the secret is shown once). Exchange them at POST https://login.backup.net/connect/token with grant_type=client_credentials (HTTP Basic client_id:client_secret), then pass the access_token as "Authorization: Bearer {token}".'
  discovery: https://login.backup.net/.well-known/openid-configuration
  docs: https://help.unitrends.kaseya.com/uniview-help/Content/MSP/public-api.htm
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.backup.net/connect/token
  name: UniView Portal OAuth 2.0 client credentials
  type: oauth2
- api: Unitrends appliance REST API (Recovery Series / Unitrends Backup)
  description: POST /api/login with the username and password of a valid system user returns an auth_token (with a timeout in seconds) that must be passed in the HTTP header of every subsequent appliance REST API request; POST /api/logout ends the session.
  docs: https://github.com/Unitrends/unitrends-api-doc/wiki/Login
  name: Appliance session token
  type: session-token
slug: unitrends-authentication
source_filename: unitrends-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/unitrends-public-api-openapi.json\ndocs: https://help.unitrends.kaseya.com/uniview-help/Content/MSP/public-api.htm\nsummary:\n  types:\n  - oauth2\n  - http-bearer\n  - session-token\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'JWT Authorization header using the Bearer scheme. Example value: \"Bearer {token}\"'\n  sources:\n  - openapi/unitrends-public-api-openapi.json\n- name: UniView Portal OAuth 2.0 client credentials\n  type: oauth2\n  api: Unitrends MSP Public API (UniView Portal)\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.backup.net/connect/token\n  discovery: https://login.backup.net/.well-known/openid-configuration\n  client_auth_methods:\n  - client_secret_post\n  - private_key_jwt\n  - client_secret_basic\n  credential_issuance: >-\n    Create public API credentials in the UniView Portal\
  \ (API Access view >\n    + New); the portal issues a Client ID and Client Secret (the secret is\n    shown once). Exchange them at POST https://login.backup.net/connect/token\n    with grant_type=client_credentials (HTTP Basic client_id:client_secret),\n    then pass the access_token as \"Authorization: Bearer {token}\".\n  docs: https://help.unitrends.kaseya.com/uniview-help/Content/MSP/public-api.htm\n- name: Appliance session token\n  type: session-token\n  api: Unitrends appliance REST API (Recovery Series / Unitrends Backup)\n  description: >-\n    POST /api/login with the username and password of a valid system user\n    returns an auth_token (with a timeout in seconds) that must be passed in\n    the HTTP header of every subsequent appliance REST API request; POST\n    /api/logout ends the session.\n  docs: https://github.com/Unitrends/unitrends-api-doc/wiki/Login\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/authentication/unitrends-authentication.yml
summary_line: oauth2/http-bearer/session-token · 3 schemes
tags:
- Company
- Backup
- Disaster Recovery
- Data Protection
- BCDR
- Ransomware Protection
- MSP
- Endpoint Backup
---
