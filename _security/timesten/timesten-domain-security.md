---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: timesten.com
  spf: true
  spf_record: v=spf1 -all
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.oracle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: www.timesten.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: redirects (301) into www.oracle.com; legacy company domain
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Timesten Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TimesTen, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TimesTen
provider_slug: timesten
slug: timesten-domain-security
source_filename: timesten-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.timesten.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: redirects (301) into www.oracle.com; legacy company domain\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: timesten.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 -all\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timesten/refs/heads/main/security/timesten-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Databases
- In-Memory Database
- Relational Databases
- Caching
- Oracle
- Acquired
---
