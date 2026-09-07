---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 3srobotics.com
  spf: true
hosts:
- cert_expires: Sep 20 04:59:59 2026 GMT
  host: 3srobotics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 3Srobotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3S robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 3S robotics
provider_slug: 3srobotics
slug: 3srobotics-domain-security
source_filename: 3srobotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 3srobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 04:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: 3srobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3srobotics/refs/heads/main/security/3srobotics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Robotics
- Industrial Robots
- Manufacturing
- Machine Vision
- Welding Automation
- Industrial Automation
- Hardware
---
