---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 83sciences.ai
  spf: true
hosts:
- cert_expires: Sep 23 02:17:04 2026 GMT
  host: 83sciences.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 83 Sciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 83 Sciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 83 Sciences
provider_slug: 83-sciences
slug: 83-sciences-domain-security
source_filename: 83-sciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 83sciences.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 02:17:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 83sciences.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/83-sciences/refs/heads/main/security/83-sciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Materials Science
- Artificial Intelligence
- Research Data
- Scientific Discovery
- Life Sciences
- Machine Learning
---
