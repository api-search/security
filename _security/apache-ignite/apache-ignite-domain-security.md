---
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
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:root@apache.org"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: ignite.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Ignite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Ignite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Ignite
provider_slug: apache-ignite
slug: apache-ignite-domain-security
source_filename: apache-ignite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ignite.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-ignite/refs/heads/main/security/apache-ignite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open-Source
- SQL
---
