---
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
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:root@apache.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: apache.local
  spf: false
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: airflow.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: apache.local
  https: false
kind: domain-security
layout: security
method: probed
name: Apache Airflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Airflow, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Airflow
provider_slug: apache-airflow
slug: apache-airflow-domain-security
source_filename: apache-airflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airflow.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apache.local\n  https: false\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: apache.local\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/security/apache-airflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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
