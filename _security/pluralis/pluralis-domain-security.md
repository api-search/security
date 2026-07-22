---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pluralis.ai
  spf: false
hosts:
- cert_expires: Sep 20 05:23:52 2026 GMT
  host: pluralis.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pluralis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pluralis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Pluralis
provider_slug: pluralis
slug: pluralis-domain-security
source_filename: pluralis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pluralis.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:23:52 2026 GMT\n  hsts: false\ndomains:\n- domain: pluralis.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pluralis/refs/heads/main/security/pluralis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Distributed Training
- Decentralized AI
- Model Parallelism
- Research
- Open Source
---
