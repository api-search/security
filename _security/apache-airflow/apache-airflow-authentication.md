---
api_key_in: []
api_specs:
- filename: apache-airflow-openapi.yaml
  format: yaml
  label: Apache Airflow REST API
  slug: apache-airflow-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/openapi/apache-airflow-openapi.yaml
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
