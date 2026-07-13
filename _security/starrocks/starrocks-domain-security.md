---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:open@starrocks.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: false
  domain: starrocks.io
  spf: false
hosts:
- cert_expires: Aug 10 01:13:41 2026 GMT
  host: www.starrocks.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: docs.starrocks.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Starrocks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StarRocks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: StarRocks
provider_slug: starrocks
slug: starrocks-domain-security
source_filename: starrocks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.starrocks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 01:13:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.starrocks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: starrocks.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:open@starrocks.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starrocks/refs/heads/main/security/starrocks-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- OLAP
- Lakehouse
- SQL
- Open Source
- Real-Time Analytics
---
