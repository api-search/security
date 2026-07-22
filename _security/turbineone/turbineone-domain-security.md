---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: turbineone.com
  spf: true
hosts:
- cert_expires: Oct 17 23:32:19 2026 GMT
  host: www.turbineone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Turbineone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TurbineOne, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TurbineOne
provider_slug: turbineone
slug: turbineone-domain-security
source_filename: turbineone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.turbineone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:32:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: turbineone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turbineone/refs/heads/main/security/turbineone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Defense
- Edge AI
- Computer Vision
- Machine Learning
- National Security
- Autonomy
---
