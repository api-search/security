---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: neros.tech
  spf: true
hosts:
- cert_expires: Oct  1 07:00:48 2026 GMT
  host: www.neros.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neros Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neros, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Neros
provider_slug: neros
slug: neros-domain-security
source_filename: neros-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neros.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 07:00:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: neros.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neros/refs/heads/main/security/neros-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Defense
- Drones
- Unmanned Systems
- UAV
- Aerospace
- Robotics
- Hardware
- Manufacturing
- Protocols
- Open Source
- Embedded
---
