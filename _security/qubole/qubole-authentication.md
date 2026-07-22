---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Qubole Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qubole secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qubole
provider_slug: qubole
scheme_count: 1
schemes:
- description: All Qubole Data Service (QDS) REST API calls are authenticated with a per-user Qubole API token sent in the X-AUTH-TOKEN request header. The token is retrieved from the Control Panel "My Accounts" tab and is commonly exported to the AUTH_TOKEN environment variable for use by the SDKs and the qds.py CLI. Confirmed in the official Python SDK (QuboleAuth.__call__ sets r.headers['X-AUTH-TOKEN']).
  in: header
  name: QuboleApiToken
  parameter_name: X-AUTH-TOKEN
  sources:
  - https://docs.qubole.com/en/latest/rest-api/
  - https://github.com/qubole/qds-sdk-py/blob/master/qds_sdk/qubole.py
  type: apiKey
slug: qubole-authentication
source_filename: qubole-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.qubole.com/en/latest/rest-api/ + github.com/qubole/qds-sdk-py (connection.py, qubole.py)\ndocs: https://docs.qubole.com/en/latest/rest-api/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: QuboleApiToken\n  type: apiKey\n  in: header\n  parameter_name: X-AUTH-TOKEN\n  description: >-\n    All Qubole Data Service (QDS) REST API calls are authenticated with a per-user\n    Qubole API token sent in the X-AUTH-TOKEN request header. The token is retrieved\n    from the Control Panel \"My Accounts\" tab and is commonly exported to the AUTH_TOKEN\n    environment variable for use by the SDKs and the qds.py CLI. Confirmed in the\n    official Python SDK (QuboleAuth.__call__ sets r.headers['X-AUTH-TOKEN']).\n  sources:\n  - https://docs.qubole.com/en/latest/rest-api/\n  - https://github.com/qubole/qds-sdk-py/blob/master/qds_sdk/qubole.py\nnotes: >-\n  Token-based (API key)\
  \ auth only; no OAuth2/OIDC scope surface is published, so no\n  scopes/ artifact is emitted. Access control is managed server-side via Qubole\n  users, groups, roles, and object-level policies. HTTPS is enforced (all HTTP is\n  redirected to HTTPS).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qubole/refs/heads/main/authentication/qubole-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data
- Data Lake
- Big Data
- Analytics
- Spark
- Presto
- Hive
- Airflow
- Machine Learning
- Cloud
- Data Engineering
---
