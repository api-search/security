---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Appneta Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppNeta secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AppNeta
provider_slug: appneta
scheme_count: 1
schemes:
- description: 'AppNeta API requests are authenticated with an API access token passed in the Authorization request header with the literal scheme word "Token", e.g. `Authorization: Token <token>`. Access tokens are the documented and recommended authentication method for API v3 and v4; they give greater control than basic authentication with a username and password, and single sign-on users can use them without a local account.'
  example_request: 'curl -X GET -H "Authorization: Token <token>" -H "Accept: application/json" "https://<application_cluster>.pm.appneta.com/api/v3/path"'
  header_name: Authorization
  in: header
  name: ApiAccessToken
  sources:
  - docs
  type: apiKey
  value_format: Token <api_access_token>
slug: appneta-authentication
source_filename: appneta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: searched\nsource: https://techdocs.broadcom.com/us/en/ca-enterprise-software/it-operations-management/appneta/GA/integrate/api/api-access-tokens.html\ndocs: https://techdocs.broadcom.com/us/en/ca-enterprise-software/it-operations-management/appneta/GA/integrate/api/api-access-tokens.html\nnote: >-\n  Re-verified 2026-09-16. The prior source URL (.../integrate/api-access-tokens.html)\n  now returns 404; the page moved under .../integrate/api/. No public OpenAPI is\n  available to derive securitySchemes from (the interactive OpenAPI 3.0 interface is\n  served per application cluster and returns 401 anonymously), so this profile is\n  taken from the TechDocs pages for API v3, API v4 and API Access Tokens.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: ApiAccessToken\n  type: apiKey\n  in: header\n  header_name: Authorization\n  value_format: Token <api_access_token>\n  description: >-\n    AppNeta API\
  \ requests are authenticated with an API access token passed in the\n    Authorization request header with the literal scheme word \"Token\", e.g.\n    `Authorization: Token <token>`. Access tokens are the documented and recommended\n    authentication method for API v3 and v4; they give greater control than basic\n    authentication with a username and password, and single sign-on users can use\n    them without a local account.\n  example_request: >-\n    curl -X GET -H \"Authorization: Token <token>\" -H \"Accept: application/json\"\n    \"https://<application_cluster>.pm.appneta.com/api/v3/path\"\n  sources: [docs]\ntoken_management:\n  created_in: AppNeta > Manage Access Tokens > Create Token\n  shown_once: true\n  expiry: configurable expiration date or Never; revoked automatically at expiration\n  expiry_notification: email two weeks before a token expires\n  scoping:\n  - role/permissions less than or equal to the creating user's permissions\n  - organization membership, either\
  \ a static selection or dynamic membership\n  immutable: true\n  revocation:\n  - manual revoke by the creator or an Organization Admin\n  - automatic at expiration\n  - automatic when the creating user is deleted\n  limitations:\n  - not available to users with custom roles\n  - /v3/observer endpoints require a token with dynamic organization membership\n  docs: https://techdocs.broadcom.com/us/en/ca-enterprise-software/it-operations-management/appneta/GA/integrate/api/api-access-tokens.html\nother_surfaces:\n- api: Monitoring Point Admin API\n  auth: interactive Swagger UI on the Monitoring Point (https://<hostname-or-ip>/swagger/index.html), reachable only from the Monitoring Point's local network or via Web Admin\n  docs: https://techdocs.broadcom.com/us/en/ca-enterprise-software/it-operations-management/appneta/GA/integrate/api/monitoring-point-admin-api.html\n- api: AppNeta On-Prem Admin API\n  auth: AppNeta login with a user that holds the System Config add-on privilege (https://<on-prem-host>/admin)\n\
  \  docs: https://techdocs.broadcom.com/us/en/ca-enterprise-software/it-operations-management/appneta/GA/integrate/api/api-on-prem.html\nerror_codes:\n- {status: 401, message: Full authentication is required to access this resource, meaning: no credentials were passed}\n- {status: 401, message: Bad credentials, meaning: credentials were passed but are invalid}\n- {status: 401, message: Failed to decode basic authentication token, meaning: an encoded token could not be decoded; recreate the token}\n- {status: 403, message: Access is denied, meaning: no permission for the resource, e.g. the wrong organization}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appneta/refs/heads/main/authentication/appneta-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Network Monitoring
- Network Performance Monitoring
- Observability
- Application Performance Monitoring
- Synthetic Monitoring
- Monitoring
- Broadcom
---
