---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iposignal.xyz
  spf: false
hosts:
- cert_expires: Jan 27 11:27:55 2027 GMT
  host: iposignal.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IPOSignal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IPOSignal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: IPOSignal
provider_slug: iposignal-xyz
slug: iposignal-xyz-domain-security
source_filename: iposignal-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iposignal.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 11:27:55 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iposignal.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/iposignal-xyz/security/iposignal-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Data
- Analytics
- IPO
- Research
---
