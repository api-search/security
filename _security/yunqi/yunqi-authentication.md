---
api_key_in: []
auth_types:
- username-password
- key-pair
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Yunqi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yunqi (ClickZetta / Singdata Lakehouse) secures its APIs with username-password, key-pair, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Yunqi (ClickZetta / Singdata Lakehouse)
provider_slug: yunqi
scheme_count: 3
schemes:
- detail: jdbc:clickzetta://{jdbcurl}/{workspace}?username={username}&password={password} — connect to a workspace on a named instance/virtual cluster.
  name: JDBC username/password
  source: https://www.yunqi.tech/documents/java_reference/jdbc
  type: connection-string
- detail: clickzetta.connect(username, password, service, instance, workspace, schema, vcluster) — the Python connector authenticates with account credentials and targets a service/instance/workspace/virtual-cluster.
  name: Python connector credentials
  source: https://www.yunqi.tech/documents/python_reference/connector
  type: connection-params
- detail: Interactive users authenticate through the ClickZetta account service at accounts.clickzetta.com (register/login); the console is an OAuth/OIDC protected SPA.
  name: Console OAuth / OIDC
  source: https://accounts.clickzetta.com/login
  type: oauth2
slug: yunqi-authentication
source_filename: yunqi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.yunqi.tech/documents/python_reference/connector + JDBC guide\nnote: >-\n  ClickZetta Lakehouse is accessed via SQL over JDBC / the Python connector /\n  ZettaPark rather than a public REST API, so there is no OpenAPI securitySchemes\n  block to derive from. This profile is captured from the SDK/driver connection\n  docs.\nsummary:\n  types: [username-password, key-pair, oauth2]\n  transport: [jdbc, python-connector, zettapark, http-console]\nschemes:\n- name: JDBC username/password\n  type: connection-string\n  detail: >-\n    jdbc:clickzetta://{jdbcurl}/{workspace}?username={username}&password={password}\n    — connect to a workspace on a named instance/virtual cluster.\n  source: https://www.yunqi.tech/documents/java_reference/jdbc\n- name: Python connector credentials\n  type: connection-params\n  detail: >-\n    clickzetta.connect(username, password, service, instance, workspace, schema,\n    vcluster) — the\
  \ Python connector authenticates with account credentials and\n    targets a service/instance/workspace/virtual-cluster.\n  source: https://www.yunqi.tech/documents/python_reference/connector\n- name: Console OAuth / OIDC\n  type: oauth2\n  detail: >-\n    Interactive users authenticate through the ClickZetta account service at\n    accounts.clickzetta.com (register/login); the console is an OAuth/OIDC\n    protected SPA.\n  source: https://accounts.clickzetta.com/login\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yunqi/refs/heads/main/authentication/yunqi-authentication.yml
summary_line: username-password/key-pair/oauth2 · 3 schemes
tags:
- Company
- Data
- Lakehouse
- Analytics
- SQL
- Cloud
- Data Engineering
- AI
- Apache Iceberg
- Database
---
