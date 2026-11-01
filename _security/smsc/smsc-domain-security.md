---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: smsc.ru
  spf: true
hosts:
- cert_expires: Apr  4 09:01:14 2027 GMT
  host: smsc.ru
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Smsc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMSC.ru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SMSC.ru
provider_slug: smsc
slug: smsc-domain-security
source_filename: smsc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smsc.ru\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  4 09:01:14 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: smsc.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/smsc/security/smsc-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- SMS
- Messaging
- Telecommunications
- API
- Russia
---
