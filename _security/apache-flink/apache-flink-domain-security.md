---
api_specs:
- filename: apache-flink-cluster-api-openapi.yml
  format: yaml
  label: Apache Flink Cluster API
  slug: apache-flink-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/openapi/apache-flink-cluster-api-openapi.yml
- filename: apache-flink-config-api-openapi.yml
  format: yaml
  label: Apache Flink Config API
  slug: apache-flink-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/openapi/apache-flink-config-api-openapi.yml
- filename: apache-flink-datasets-api-openapi.yml
  format: yaml
  label: Apache Flink Datasets API
  slug: apache-flink-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/openapi/apache-flink-datasets-api-openapi.yml
- filename: apache-flink-jars-api-openapi.yml
  format: yaml
  label: Apache Flink Jars API
  slug: apache-flink-jars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/openapi/apache-flink-jars-api-openapi.yml
- filename: apache-flink-jobmanager-api-openapi.yml
  format: yaml
  label: Apache Flink Jobmanager API
  slug: apache-flink-jobmanager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/openapi/apache-flink-jobmanager-api-openapi.yml
- filename: apache-flink-jobs-api-openapi.yml
  format: yaml
  label: Apache Flink Jobs API
  slug: apache-flink-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/openapi/apache-flink-jobs-api-openapi.yml
- filename: apache-flink-overview-api-openapi.yml
  format: yaml
  label: Apache Flink Overview API
  slug: apache-flink-overview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/openapi/apache-flink-overview-api-openapi.yml
- filename: apache-flink-savepoint-disposal-api-openapi.yml
  format: yaml
  label: Apache Flink Savepoint Disposal API
  slug: apache-flink-savepoint-disposal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/openapi/apache-flink-savepoint-disposal-api-openapi.yml
- filename: apache-flink-taskmanagers-api-openapi.yml
  format: yaml
  label: Apache Flink Taskmanagers API
  slug: apache-flink-taskmanagers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/openapi/apache-flink-taskmanagers-api-openapi.yml
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
hosts:
- cert_expires: Sep 27 08:45:06 2026 GMT
  host: nightlies.apache.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Flink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Flink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Flink
provider_slug: apache-flink
slug: apache-flink-domain-security
source_filename: apache-flink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nightlies.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 08:45:06 2026 GMT\n  hsts: false\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/security/apache-flink-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
---
