---
api_key_in: []
api_specs:
- filename: apache-airflow-config-api-openapi.yml
  format: yaml
  label: Apache Airflow Config API
  slug: apache-airflow-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-config-api-openapi.yml
- filename: apache-airflow-connection-api-openapi.yml
  format: yaml
  label: Apache Airflow Connection API
  slug: apache-airflow-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-connection-api-openapi.yml
- filename: apache-airflow-dag-api-openapi.yml
  format: yaml
  label: Apache Airflow DAG API
  slug: apache-airflow-dag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-dag-api-openapi.yml
- filename: apache-airflow-dagrun-api-openapi.yml
  format: yaml
  label: Apache Airflow DAGRun API
  slug: apache-airflow-dagrun-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-dagrun-api-openapi.yml
- filename: apache-airflow-dagwarning-api-openapi.yml
  format: yaml
  label: Apache Airflow DagWarning API
  slug: apache-airflow-dagwarning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-dagwarning-api-openapi.yml
- filename: apache-airflow-dataset-api-openapi.yml
  format: yaml
  label: Apache Airflow Dataset API
  slug: apache-airflow-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-dataset-api-openapi.yml
- filename: apache-airflow-eventlog-api-openapi.yml
  format: yaml
  label: Apache Airflow EventLog API
  slug: apache-airflow-eventlog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-eventlog-api-openapi.yml
- filename: apache-airflow-importerror-api-openapi.yml
  format: yaml
  label: Apache Airflow ImportError API
  slug: apache-airflow-importerror-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-importerror-api-openapi.yml
- filename: apache-airflow-monitoring-api-openapi.yml
  format: yaml
  label: Apache Airflow Monitoring API
  slug: apache-airflow-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-monitoring-api-openapi.yml
- filename: apache-airflow-permission-api-openapi.yml
  format: yaml
  label: Apache Airflow Permission API
  slug: apache-airflow-permission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-permission-api-openapi.yml
- filename: apache-airflow-plugin-api-openapi.yml
  format: yaml
  label: Apache Airflow Plugin API
  slug: apache-airflow-plugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-plugin-api-openapi.yml
- filename: apache-airflow-pool-api-openapi.yml
  format: yaml
  label: Apache Airflow Pool API
  slug: apache-airflow-pool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-pool-api-openapi.yml
- filename: apache-airflow-provider-api-openapi.yml
  format: yaml
  label: Apache Airflow Provider API
  slug: apache-airflow-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-provider-api-openapi.yml
- filename: apache-airflow-role-api-openapi.yml
  format: yaml
  label: Apache Airflow Role API
  slug: apache-airflow-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-role-api-openapi.yml
- filename: apache-airflow-taskinstance-api-openapi.yml
  format: yaml
  label: Apache Airflow TaskInstance API
  slug: apache-airflow-taskinstance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-taskinstance-api-openapi.yml
- filename: apache-airflow-user-api-openapi.yml
  format: yaml
  label: Apache Airflow User API
  slug: apache-airflow-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-user-api-openapi.yml
- filename: apache-airflow-variable-api-openapi.yml
  format: yaml
  label: Apache Airflow Variable API
  slug: apache-airflow-variable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-variable-api-openapi.yml
- filename: apache-airflow-xcom-api-openapi.yml
  format: yaml
  label: Apache Airflow XCom API
  slug: apache-airflow-xcom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-xcom-api-openapi.yml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Apache Airflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Airflow secures its APIs with http and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Apache Airflow
provider_slug: apache-airflow
scheme_count: 3
schemes:
- name: Basic
  scheme: basic
  sources:
  - openapi/apache-airflow-openapi.yaml
  type: http
- name: GoogleOpenId
  openIdConnectUrl: https://accounts.google.com/.well-known/openid-configuration
  sources:
  - openapi/apache-airflow-openapi.yaml
  type: openIdConnect
- name: Kerberos
  scheme: negotiate
  sources:
  - openapi/apache-airflow-openapi.yaml
  type: http
slug: apache-airflow-authentication
source_filename: apache-airflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-airflow-openapi.yaml\nsummary:\n  types:\n  - http\n  - openIdConnect\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/apache-airflow-openapi.yaml\n- name: GoogleOpenId\n  type: openIdConnect\n  openIdConnectUrl: https://accounts.google.com/.well-known/openid-configuration\n  sources:\n  - openapi/apache-airflow-openapi.yaml\n- name: Kerberos\n  type: http\n  scheme: negotiate\n  sources:\n  - openapi/apache-airflow-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/authentication/apache-airflow-authentication.yml
summary_line: http/openIdConnect · 3 schemes
tags:
- Apache
- DAG
- Data Pipeline
- ETL
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
---
