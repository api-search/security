---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Airspace Link Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Airspace Link secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Airspace Link
provider_slug: airspace-link
scheme_count: 2
schemes:
- flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  request_content_type: application/x-www-form-urlencoded
  request_params:
  - grant_type
  - client_id
  - client_secret
  - scope
  sent_in: Authorization header
  sources:
  - searched:doc-2002712
  - searched:api-31492994
  tokenUrl: https://airhub-api-sandbox.airspacelink.com/v1/oauth/token
  token_field: data.accessToken
  type: oauth2
- in: header
  name: x-api-key
  required: true
  sources:
  - searched:doc-2002712
  type: apiKey
slug: airspace-link-authentication
source_filename: airspace-link-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.airspacelink.com/doc-2002712\ndocs: https://developers.airspacelink.com/doc-2002712\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  api_key_name: x-api-key\n  oauth2_flows: [clientCredentials]\nnotes: >-\n  AirHub API requires BOTH an OAuth 2.0 client-credentials access token (sent in\n  the Authorization header) AND an x-api-key header on every request. Client id\n  and client secret are supplied by Airspace Link (not self-service). The OAuth\n  token response is wrapped in the standard AirHub envelope\n  ({ data: { accessToken, expires }, message, statusCode }).\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://airhub-api-sandbox.airspacelink.com/v1/oauth/token\n  grant_type: client_credentials\n  request_content_type: application/x-www-form-urlencoded\n  request_params: [grant_type, client_id, client_secret, scope]\n  token_field:\
  \ data.accessToken\n  sent_in: Authorization header\n  sources: [searched:doc-2002712, searched:api-31492994]\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  name: x-api-key\n  required: true\n  sources: [searched:doc-2002712]\nenvironments:\n  sandbox: https://airhub-api-sandbox.airspacelink.com\n  live: https://airhub-api.airspacelink.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airspace-link/refs/heads/main/authentication/airspace-link-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Drones
- UAS
- Airspace
- Aviation
- LAANC
- UTM
- Geospatial
- Public Safety
- Logistics
---
