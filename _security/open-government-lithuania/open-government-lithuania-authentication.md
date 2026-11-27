---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Lithuanian Open Data Portal (data.gov.lt) Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lithuanian Open Data Portal (data.gov.lt) declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lithuanian Open Data Portal (data.gov.lt)
provider_slug: open-government-lithuania
scheme_count: 2
schemes:
- applies_to: https://get.data.gov.lt (read-only open data)
  name: anonymous
  note: 'Docs: authorization is not required to get open data ("Norint gauti atvirus duomenis autorizacija nereikalinga").'
  type: none
- applies_to: https://put.data.gov.lt (write operations)
  flow: clientCredentials
  name: oauth2ClientCredentials
  note: Only the client credentials flow is currently supported; an account must be created for the client in the store first.
  tokenUrl: https://put.data.gov.lt/auth/token
  token_usage: 'Authorization: Bearer <access_token>'
  type: oauth2
slug: open-government-lithuania-authentication
source_filename: open-government-lithuania-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: searched\nsource: https://atviriduomenys.readthedocs.io/latest/api/index.html\nname: Lithuanian Open Data Portal authentication\ndocs: https://atviriduomenys.readthedocs.io/latest/api/index.html#autorizacija\nschemes:\n- name: anonymous\n  type: none\n  applies_to: https://get.data.gov.lt (read-only open data)\n  note: 'Docs: authorization is not required to get open data (\"Norint gauti atvirus\n    duomenis autorizacija nereikalinga\").'\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://put.data.gov.lt/auth/token\n  token_usage: 'Authorization: Bearer <access_token>'\n  applies_to: https://put.data.gov.lt (write operations)\n  note: Only the client credentials flow is currently supported; an account must be\n    created for the client in the store first.\n"
source_yaml_url: https://artifacts.apis.io/open-government-lithuania/authentication/open-government-lithuania-authentication.yml
summary_line: 2 schemes
tags:
- Datasets
- Government
- Lithuania
- Open Data
- Public APIs
- Public Sector
- UAPI
---
