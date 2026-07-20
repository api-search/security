---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cask Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cask secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cask
provider_slug: cask
scheme_count: 1
schemes:
- condition: required when security.enabled=true in cdap-site.xml
  format: 'Authorization: Bearer <access-token>'
  header: Authorization
  in: header
  issued_by: CDAP authentication server
  name: cdapAccessToken
  scheme: bearer
  sources:
  - https://cdap.atlassian.net/wiki/spaces/DOCS/pages/477692124/Microservices+Introduction
  type: http
slug: cask-authentication
source_filename: cask-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://cdap.atlassian.net/wiki/spaces/DOCS/pages/477692124/Microservices+Introduction\ndocs: https://cdap.atlassian.net/wiki/spaces/DOCS/pages/477692124/Microservices+Introduction\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  oauth2_flows: []\n  api_key_in: []\n  optional: true\nnotes: >-\n  Authentication on CDAP is conditional on cluster configuration. When security.enabled=true in\n  cdap-site.xml, every call to the Microservices (HTTP RESTful) API must be authenticated: the client\n  first obtains an access token from the CDAP authentication server and then supplies it on every\n  request. For CDAP-issued access tokens the authentication scheme must always be Bearer. When\n  security.authorization.enabled=true, authenticated calls are additionally authorization-checked\n  against CDAP authorization policies, and an authenticated-but-unprivileged caller receives 403.\n  An unauthenticated call against a\
  \ security-enabled cluster receives 401.\nschemes:\n- name: cdapAccessToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <access-token>'\n  issued_by: CDAP authentication server\n  condition: required when security.enabled=true in cdap-site.xml\n  sources:\n  - https://cdap.atlassian.net/wiki/spaces/DOCS/pages/477692124/Microservices+Introduction\nauthorization:\n  model: policy-based privileges on CDAP entities\n  condition: enforced when security.authorization.enabled=true in cdap-site.xml\n  failure_status: 403\n  management_api: https://cdap.atlassian.net/wiki/spaces/DOCS/pages/477790661/Security+Microservices\ncli_credential_cache: ~/.cdap.accesstoken.<hostname>\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cask/refs/heads/main/authentication/cask-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Big Data
- Data Analytics
- Data Pipelines
- Data Integration
- ETL
- Hadoop
- Spark
- Open Source
- CDAP
- Metadata
- Data Governance
- Acquired
---
