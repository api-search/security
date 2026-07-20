---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Etleap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Etleap secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Etleap
provider_slug: etleap
scheme_count: 1
schemes:
- applies_to: All API v2 requests to https://api.etleap.com/api/v2
  name: basicAuth
  scheme: basic
  source: docs.etleap.com/docs/api-v2
  type: http
slug: etleap-authentication
source_filename: etleap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.etleap.com/docs/api-v2/d34fe805d6516-how-to-get-started\ndocs: https://docs.etleap.com/docs/api-v2\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Etleap API v2 authenticates every request with HTTP Basic authentication.\n    Credentials are an API-user's key and secret issued from the Etleap\n    application. A separate OAuth 2.0 flow (initiateOAuth2) exists only for\n    authorizing third-party source connections (e.g. Google, Salesforce), not\n    for authenticating to the Etleap API itself.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  source: docs.etleap.com/docs/api-v2\n  applies_to: All API v2 requests to https://api.etleap.com/api/v2\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/etleap/refs/heads/main/authentication/etleap-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data Integration
- ETL
- ELT
- Data Pipelines
- Data Warehouse
- Data Lake
- Apache Iceberg
- Analytics
---
