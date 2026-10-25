---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bureau Of Meteorology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bureau of Meteorology declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Bureau of Meteorology
provider_slug: bureau-of-meteorology
scheme_count: 2
schemes:
- api: Space Weather API
  description: Use of the API requires registration. Upon successful registration, an API key will be provided. This key needs to be included in requests for data. The key is sent as the api_key field of the JSON POST body (example format is a UUID).
  field: api_key
  in: body
  name: api_key_in_body
  obtain: https://sws-data.sws.bom.gov.au/register
  type: apiKey
- api: Registered User Services (real-time data feeds)
  description: Registered-user real-time data and Cloud (S)FTP services require registration; anonymous FTP and web products are free and need no credential.
  docs: https://reg.bom.gov.au/catalogue/data-feeds.shtml
  name: registered_user_services
  type: other
slug: bureau-of-meteorology-authentication
source_filename: bureau-of-meteorology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: searched\nsource: https://sws-data.sws.bom.gov.au/api-docs#overview\ndocs: https://sws-data.sws.bom.gov.au/api-docs\nschemes:\n- name: api_key_in_body\n  type: apiKey\n  in: body\n  field: api_key\n  api: Space Weather API\n  description: Use of the API requires registration. Upon successful registration, an API key will be provided. This key needs to be included in requests for data. The key is sent as the api_key field of the JSON POST body (example format is a UUID).\n  obtain: https://sws-data.sws.bom.gov.au/register\n- name: registered_user_services\n  type: other\n  api: Registered User Services (real-time data feeds)\n  description: Registered-user real-time data and Cloud (S)FTP services require registration; anonymous FTP and web products are free and need no credential.\n  docs: https://reg.bom.gov.au/catalogue/data-feeds.shtml\ntransport: HTTPS should be used for all API requests. Support for unencrypted HTTP requests will be withdrawn\
  \ in early 2022.\nnote: No OAuth or OpenID Connect is documented. The registration page was not called (probe-safety rule); its URL is taken from the docs page's own link.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-meteorology/refs/heads/main/authentication/bureau-of-meteorology-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Government
- Weather
- Climate
- Meteorology
- Water
- Open Data
- Australia
---
