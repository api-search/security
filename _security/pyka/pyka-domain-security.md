---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flypyka.com
  spf: true
hosts:
- cert_expires: Sep 28 09:33:30 2026 GMT
  host: flypyka.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pyka Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pyka, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pyka
provider_slug: pyka
slug: pyka-domain-security
source_filename: pyka-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flypyka.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 09:33:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flypyka.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pyka/refs/heads/main/security/pyka-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Autonomous Aircraft
- Drones
- Aerospace
- Agriculture
- Logistics
- Defense
- Robotics
- Electric Aviation
---
