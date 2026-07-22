---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: robocurve.org
  spf: true
hosts:
- cert_expires: Sep 24 23:44:15 2026 GMT
  host: robocurve.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Robocurve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Robocurve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Robocurve
provider_slug: robocurve
slug: robocurve-domain-security
source_filename: robocurve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: robocurve.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:44:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: robocurve.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/robocurve/refs/heads/main/security/robocurve-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Physical AI
- Evaluation
- Benchmarks
- Open Source
- Machine Learning
- Vision Language Action
---
