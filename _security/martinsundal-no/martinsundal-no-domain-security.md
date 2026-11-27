---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: martinsundal.no
  spf: true
hosts:
- cert_expires: Jan 14 15:34:37 2027 GMT
  host: martinsundal.no
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Martin Sundal Aspås Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Martin Sundal Aspås, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Martin Sundal Aspås
provider_slug: martinsundal-no
slug: martinsundal-no-domain-security
source_filename: martinsundal-no-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: martinsundal.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 15:34:37 2027 GMT\n  hsts: false\ndomains:\n- domain: martinsundal.no\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/martinsundal-no/security/martinsundal-no-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Software Engineer
- Robotics
- Simulation
- Machine Learning
- Quantum Technology
---
