---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qubole.com
  spf: true
hosts:
- cert_expires: Sep 19 06:56:51 2026 GMT
  host: www.qubole.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 06:56:51 2026 GMT
  host: docs.qubole.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 06:56:51 2026 GMT
  host: api.qubole.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qubole Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qubole, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qubole
provider_slug: qubole
slug: qubole-domain-security
source_filename: qubole-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qubole.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 06:56:51 2026 GMT\n  hsts: false\n- host: docs.qubole.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 06:56:51 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: api.qubole.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 06:56:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qubole.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qubole/refs/heads/main/security/qubole-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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
