---
anonymous_access: true
api_key_in: []
api_specs:
- filename: data-gov-au-openapi-generated.yml
  format: yaml
  label: data.gov.au Federal API
  slug: data-gov-au-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/data-gov-au/refs/heads/main/openapi/_ae-authored/data-gov-au-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Data Gov Au Authentication
name_suffix: Authentication
oauth_flows: []
overview: data.gov.au Federal declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: data.gov.au Federal
provider_slug: data-gov-au
scheme_count: 2
schemes:
- description: GET-able API functions (ckan.logic.action.get), e.g. package_list and package_search, can be called without authentication.
  name: anonymous
  type: none
- description: '"To provide your API token in an HTTP request, include it in an Authorization header." The header name is configurable per site via the apitoken_header_name option.'
  example: 'curl -H "Authorization: XXX"  https://demo.ckan.org/api/3/action/am_following_user?id=markw'
  header: Authorization
  in: header
  name: apiToken
  type: apiKey
slug: data-gov-au-authentication
source_filename: data-gov-au-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource: https://docs.ckan.org/en/latest/api/\ndocs: https://docs.ckan.org/en/latest/api/#authentication-and-api-tokens\nnote: >-\n  data.gov.au publishes no OpenAPI and no API page of its own; apis.yml points its Documentation at the CKAN platform\n  docs (docs.ckan.org), which this profile is read from. Site-specific configuration (for example a renamed token\n  header) could not be checked: data.gov.au answered 503 with \"Data.gov.au is currently undergoing maintenance. We'll\n  be back online on 22 October 2026.\" on 2026-10-21.\nsummary: >-\n  Read (GET-able) actions need no credentials. Actions that require authorization take a CKAN API token in the\n  Authorization header; tokens are generated in the UI (User Profile > Manage > API tokens) or via api_token_create,\n  can be revoked at any time, and can be given an expiry when the expire_api_token plugin is enabled.\nschemes:\n- name: anonymous\n  type: none\n  description: GET-able\
  \ API functions (ckan.logic.action.get), e.g. package_list and package_search, can be called without authentication.\n- name: apiToken\n  type: apiKey\n  in: header\n  header: Authorization\n  description: >-\n    \"To provide your API token in an HTTP request, include it in an Authorization header.\" The header name is\n    configurable per site via the apitoken_header_name option.\n  example: 'curl -H \"Authorization: XXX\"  https://demo.ckan.org/api/3/action/am_following_user?id=markw'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-gov-au/refs/heads/main/authentication/data-gov-au-authentication.yml
summary_line: 2 schemes
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- National Government
- Australia
- Federal Government
- Public Sector
---
