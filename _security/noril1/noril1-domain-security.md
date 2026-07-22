---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: norirobotics.com
  spf: true
hosts:
- cert_expires: Sep 21 16:26:50 2026 GMT
  host: www.norirobotics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 22:01:52 2026 GMT
  host: docs.norirobotics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noril1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nori, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Nori
provider_slug: noril1
slug: noril1-domain-security
source_filename: noril1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.norirobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:26:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.norirobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 22:01:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: norirobotics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noril1/refs/heads/main/security/noril1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Robotics
- Humanoid Robots
- Teleoperation
- SDK
- WebRTC
- Hardware
- Home Automation
- Developer Tools
- Y Combinator
---
