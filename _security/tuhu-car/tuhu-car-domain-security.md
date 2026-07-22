---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tuhu.cn
  spf: true
hosts:
- cert_expires: Jan 18 08:06:02 2027 GMT
  host: tuhu.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tuhu Car Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tuhu Car, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tuhu Car
provider_slug: tuhu-car
slug: tuhu-car-domain-security
source_filename: tuhu-car-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tuhu.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 18 08:06:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tuhu.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tuhu-car/refs/heads/main/security/tuhu-car-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Consumer
- Automotive
- Car Maintenance
- Aftermarket Services
---
