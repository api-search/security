---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: betternight.com
  spf: true
hosts:
- cert_expires: Oct  5 04:24:13 2026 GMT
  host: betternight.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: sleep.betternight.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: admin.betternight.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 11 12:22:53 2026 GMT
  host: www.support.betternight.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Betternight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BetterNight, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BetterNight
provider_slug: betternight
slug: betternight-domain-security
source_filename: betternight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: betternight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 04:24:13 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: sleep.betternight.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\n- host: admin.betternight.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\n- host: www.support.betternight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 12:22:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: betternight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betternight/refs/heads/main/security/betternight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Digital Health
- Telehealth
- Sleep Health
- Sleep Apnea
- Remote Patient Monitoring
- Medical Devices
- Virtual Care
---
