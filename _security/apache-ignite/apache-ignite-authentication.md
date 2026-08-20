---
api_key_in: []
api_specs:
- filename: apache-ignite-clusterconfiguration-api-openapi.yml
  format: yaml
  label: Apache Ignite clusterConfiguration API
  slug: apache-ignite-clusterconfiguration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/openapi/apache-ignite-clusterconfiguration-api-openapi.yml
- filename: apache-ignite-clustermanagement-api-openapi.yml
  format: yaml
  label: Apache Ignite clusterManagement API
  slug: apache-ignite-clustermanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/openapi/apache-ignite-clustermanagement-api-openapi.yml
- filename: apache-ignite-clustermetric-api-openapi.yml
  format: yaml
  label: Apache Ignite clusterMetric API
  slug: apache-ignite-clustermetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/openapi/apache-ignite-clustermetric-api-openapi.yml
- filename: apache-ignite-compute-api-openapi.yml
  format: yaml
  label: Apache Ignite compute API
  slug: apache-ignite-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/openapi/apache-ignite-compute-api-openapi.yml
- filename: apache-ignite-deployment-api-openapi.yml
  format: yaml
  label: Apache Ignite deployment API
  slug: apache-ignite-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/openapi/apache-ignite-deployment-api-openapi.yml
- filename: apache-ignite-nodeconfiguration-api-openapi.yml
  format: yaml
  label: Apache Ignite nodeConfiguration API
  slug: apache-ignite-nodeconfiguration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/openapi/apache-ignite-nodeconfiguration-api-openapi.yml
- filename: apache-ignite-nodemanagement-api-openapi.yml
  format: yaml
  label: Apache Ignite nodeManagement API
  slug: apache-ignite-nodemanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/openapi/apache-ignite-nodemanagement-api-openapi.yml
- filename: apache-ignite-nodemetric-api-openapi.yml
  format: yaml
  label: Apache Ignite nodeMetric API
  slug: apache-ignite-nodemetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/openapi/apache-ignite-nodemetric-api-openapi.yml
- filename: apache-ignite-recovery-api-openapi.yml
  format: yaml
  label: Apache Ignite recovery API
  slug: apache-ignite-recovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/openapi/apache-ignite-recovery-api-openapi.yml
- filename: apache-ignite-sql-api-openapi.yml
  format: yaml
  label: Apache Ignite sql API
  slug: apache-ignite-sql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/openapi/apache-ignite-sql-api-openapi.yml
- filename: apache-ignite-system-api-openapi.yml
  format: yaml
  label: Apache Ignite system API
  slug: apache-ignite-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/openapi/apache-ignite-system-api-openapi.yml
- filename: apache-ignite-topology-api-openapi.yml
  format: yaml
  label: Apache Ignite topology API
  slug: apache-ignite-topology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/openapi/apache-ignite-topology-api-openapi.yml
- filename: apache-ignite-transactions-api-openapi.yml
  format: yaml
  label: Apache Ignite transactions API
  slug: apache-ignite-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/openapi/apache-ignite-transactions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apache Ignite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apache Ignite secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apache Ignite
provider_slug: apache-ignite
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/apache-ignite-rest-api.yaml
  type: http
slug: apache-ignite-authentication
source_filename: apache-ignite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-ignite-rest-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/apache-ignite-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/authentication/apache-ignite-authentication.yml
summary_line: http · 1 scheme
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open-Source
- SQL
---
