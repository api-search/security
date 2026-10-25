---
anonymous_access: false
api_key_in: []
api_specs:
- filename: anaplaninc
  format: yaml
  label: Anaplan Integration API v2.0
  slug: anaplan-integration-api-v2-0
  spec_type: Postman
  url: https://www.postman.com/anaplaninc
- filename: anaplan-openapi-generated.yml
  format: yaml
  label: Anaplan API
  slug: anaplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anaplan/refs/heads/main/openapi/_ae-authored/anaplan-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Anaplan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anaplan declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Anaplan
provider_slug: anaplan
scheme_count: 3
schemes:
- description: Username and password sent as Basic auth to POST /token/authenticate to obtain an Anaplan auth token.
  scheme: basic
  type: http
- description: 'All API calls send "Authorization: AnaplanAuthToken {token}"; tokens are refreshed with /token/refresh, inspected with /token/validate and deleted with /token/logout.'
  in: header
  name: Authorization
  type: apiKey
- description: CA-issued client certificate authentication against /token/authenticate as an alternative to username/password.
  type: certificate
slug: anaplan-authentication
source_filename: anaplan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Anaplan authentication\ngenerated: '2026-10-20'\nmethod: searched\nsource: https://anaplanauthentication.docs.apiary.io/\ndocs: https://help.anaplan.com/authentication-service-api-4060eddf-fe4e-4220-96f6-267d54502ed6\ntoken_endpoint: https://auth.anaplan.com/token/authenticate\nschemes:\n- type: http\n  scheme: basic\n  description: Username and password sent as Basic auth to POST /token/authenticate to obtain an Anaplan auth token.\n- type: apiKey\n  in: header\n  name: Authorization\n  description: 'All API calls send \"Authorization: AnaplanAuthToken {token}\"; tokens are refreshed with /token/refresh, inspected with /token/validate and deleted with /token/logout.'\n- type: certificate\n  description: CA-issued client certificate authentication against /token/authenticate as an alternative to username/password.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anaplan/refs/heads/main/authentication/anaplan-authentication.yml
summary_line: 3 schemes
tags:
- Connected Planning
- Enterprise Planning
- FP&A
- Supply Chain
- Sales Planning
- Financial Consolidation
- SCIM
- REST
---
