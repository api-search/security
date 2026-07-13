---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Oracle Database REST API - Partitioning
  slug: oracle-database-rest-api-partitioning
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/
- filename: database.json
  format: json
  label: Oracle Cloud Infrastructure Database API - Partitioning
  slug: oracle-cloud-infrastructure-database-api-partitioning
  spec_type: OpenAPI
  url: https://docs.oracle.com/en-us/iaas/api/swagger/database.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your-oracle-instance.com
  spf: false
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.oracle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: your-oracle-instance.com
  https: false
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.oracle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle Partitioning Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Partitioning, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Partitioning
provider_slug: oracle-partitioning
slug: oracle-partitioning-domain-security
source_filename: oracle-partitioning-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: your-oracle-instance.com\n  https: false\n- host: www.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: your-oracle-instance.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-partitioning/refs/heads/main/security/oracle-partitioning-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Composite-Partitioning
- Database
- Hash-Partitioning
- Interval-Partitioning
- List-Partitioning
- Oracle
- Partitioning
- Performance
- Range-Partitioning
- Scalability
- VLDB
---
