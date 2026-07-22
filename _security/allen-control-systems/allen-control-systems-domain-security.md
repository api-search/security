---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: allencontrolsystems.com
  spf: true
hosts:
- cert_expires: Oct  2 20:11:13 2026 GMT
  host: allencontrolsystems.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allen Control Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allen Control Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Allen Control Systems
provider_slug: allen-control-systems
slug: allen-control-systems-domain-security
source_filename: allen-control-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: allencontrolsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:11:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: allencontrolsystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allen-control-systems/refs/heads/main/security/allen-control-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Defense
- Counter-Drone
- Autonomous Systems
- Weapon Systems
- Robotics
- Machine Vision
- Command and Control
---
