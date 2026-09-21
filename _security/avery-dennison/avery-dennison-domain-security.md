---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: averydennison.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: atma.io
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.averydennison.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: developer.averydennison.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 23 18:39:55 2026 GMT
  host: www.atma.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Avery Dennison Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avery Dennison, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Avery Dennison
provider_slug: avery-dennison
slug: avery-dennison-domain-security
source_filename: avery-dennison-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.averydennison.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.averydennison.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: www.atma.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 18:39:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: averydennison.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: atma.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avery-dennison/refs/heads/main/security/avery-dennison-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Fortune 500
- IoT
- RFID
- Labels
- Supply Chain
- Manufacturing
- Digital Product Passport
---
