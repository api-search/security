---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issuewild "trust-provider.com"
  - 0 issuewild "usertrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: etleap.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: docs.etleap.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 04:31:24 2026 GMT
  host: api.etleap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Etleap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Etleap, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Etleap
provider_slug: etleap
slug: etleap-domain-security
source_filename: etleap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.etleap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: api.etleap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 04:31:24 2026 GMT\n  hsts: null\ndomains:\n- domain: etleap.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issuewild \"trust-provider.com\"\n  - 0 issuewild \"usertrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/etleap/refs/heads/main/security/etleap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Integration
- ETL
- ELT
- Data Pipelines
- Data Warehouse
- Data Lake
- Apache Iceberg
- Analytics
---
