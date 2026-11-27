---
anonymous_access: false
api_key_in: []
api_specs:
- filename: yunqi-analytics-agent-api-openapi.yml
  format: yaml
  label: Yunqi Analytics Agent Open API
  slug: yunqi-analytics-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yunqi/openapi/yunqi-analytics-agent-api-openapi.yml
- filename: yunqi-ai-gateway-api-openapi.yml
  format: yaml
  label: Yunqi AI Gateway API
  slug: yunqi-ai-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yunqi/openapi/yunqi-ai-gateway-api-openapi.yml
- filename: yunqi-dqc-api-openapi.yml
  format: yaml
  label: Yunqi (ClickZetta / Singdata Lakehouse) Dqc API
  slug: yunqi-dqc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yunqi/openapi/yunqi-dqc-api-openapi.yml
- filename: yunqi-instance-api-openapi.yml
  format: yaml
  label: Yunqi (ClickZetta / Singdata Lakehouse) Instance API
  slug: yunqi-instance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yunqi/openapi/yunqi-instance-api-openapi.yml
- filename: yunqi-multirealtimeditask-api-openapi.yml
  format: yaml
  label: Yunqi (ClickZetta / Singdata Lakehouse) Multi Realtime Di Task API
  slug: yunqi-multirealtimeditask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yunqi/openapi/yunqi-multirealtimeditask-api-openapi.yml
- filename: yunqi-realtimetask-api-openapi.yml
  format: yaml
  label: Yunqi (ClickZetta / Singdata Lakehouse) Realtime Task API
  slug: yunqi-realtimetask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yunqi/openapi/yunqi-realtimetask-api-openapi.yml
- filename: yunqi-scheduletask-api-openapi.yml
  format: yaml
  label: Yunqi (ClickZetta / Singdata Lakehouse) Schedule Task API
  slug: yunqi-scheduletask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yunqi/openapi/yunqi-scheduletask-api-openapi.yml
- filename: yunqi-user-management-api-openapi.yml
  format: yaml
  label: Yunqi (ClickZetta / Singdata Lakehouse) User Management API
  slug: yunqi-user-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yunqi/openapi/yunqi-user-management-api-openapi.yml
- filename: yunqi-virtualcluster-api-openapi.yml
  format: yaml
  label: Yunqi (ClickZetta / Singdata Lakehouse) Virtual Cluster API
  slug: yunqi-virtualcluster-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yunqi/openapi/yunqi-virtualcluster-api-openapi.yml
- filename: yunqi-workspace-api-openapi.yml
  format: yaml
  label: Yunqi (ClickZetta / Singdata Lakehouse) Workspace API
  slug: yunqi-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yunqi/openapi/yunqi-workspace-api-openapi.yml
- filename: yunqi-data-source-api-openapi.yml
  format: yaml
  label: Yunqi (ClickZetta / Singdata Lakehouse) Data Source API
  slug: yunqi-data-source-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yunqi/openapi/yunqi-data-source-api-openapi.yml
auth_types:
- username-password
- key-pair
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Yunqi (ClickZetta / Singdata Lakehouse) Authentication
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
source_yaml_url: https://artifacts.apis.io/yunqi/authentication/yunqi-authentication.yml
summary_line: username-password/key-pair/oauth2 · 3 schemes
tags:
- Company
- Data
- Lakehouse
- Analytics
- SQL
- Cloud
- Data Engineering
- Artificial Intelligence
- Apache Iceberg
- Database
---
