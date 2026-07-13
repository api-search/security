---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ibm.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dashdb.com
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.ibm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: cloud.ibm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.dashdb.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ibm Db2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IBM Db2, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IBM Db2
provider_slug: ibm-db2
slug: ibm-db2-domain-security
source_filename: ibm-db2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ibm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.ibm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: null\n- host: api.dashdb.com\n  https: false\ndomains:\n- domain: ibm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dashdb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibm-db2/refs/heads/main/security/ibm-db2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- Relational Database
- Cloud Database
- SQL
- Data Management
- IBM Cloud
---
