---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lucidmotors.com
  spf: true
hosts:
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: www.lucidmotors.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lucid Motors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lucid Motors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lucid Motors
provider_slug: lucid-motors
slug: lucid-motors-domain-security
source_filename: lucid-motors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lucidmotors.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: lucidmotors.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucid-motors/refs/heads/main/security/lucid-motors-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Automotive
- Electric Vehicles
- Luxury Vehicles
- Connected Vehicle
- Battery Technology
- Powertrain
- Manufacturing
- Over The Air Updates
- Mobile App
- Lucid Air
- Lucid Gravity
- NASDAQ
---
