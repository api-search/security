---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: braiins.com
  spf: true
hosts:
- cert_expires: Aug 17 01:12:51 2026 GMT
  host: braiins.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 12:23:41 2026 GMT
  host: academy.braiins.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Braiins Academy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Braiins, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Braiins
provider_slug: braiins-academy
slug: braiins-academy-domain-security
source_filename: braiins-academy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: braiins.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 01:12:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: academy.braiins.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 12:23:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: braiins.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braiins-academy/refs/heads/main/security/braiins-academy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Bitcoin Mining
- Cryptocurrency
- Mining Pool
- Mining Firmware
- Blockchain
- Stratum V2
---
