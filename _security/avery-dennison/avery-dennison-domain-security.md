---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: avery-dennison.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: averydennison.com
  spf: true
hosts:
- host: www.avery-dennison.com
  https: false
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: developer.averydennison.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Avery Dennison Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avery Dennison, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Avery Dennison
provider_slug: avery-dennison
slug: avery-dennison-domain-security
source_filename: avery-dennison-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avery-dennison.com\n  https: false\n- host: developer.averydennison.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\ndomains:\n- domain: avery-dennison.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: averydennison.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avery-dennison/refs/heads/main/security/avery-dennison-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Fortune 500
- IoT
- RFID
- Labels
- Supply Chain
- Manufacturing
---
