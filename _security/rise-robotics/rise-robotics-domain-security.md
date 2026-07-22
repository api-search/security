---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: riserobotics.com
  spf: true
hosts:
- cert_expires: Oct 10 02:16:47 2026 GMT
  host: riserobotics.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rise Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rise Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rise Robotics
provider_slug: rise-robotics
slug: rise-robotics-domain-security
source_filename: rise-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: riserobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 02:16:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: riserobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rise-robotics/refs/heads/main/security/rise-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Actuation
- Industrial
- Hardware
- Defense
- Manufacturing
---
