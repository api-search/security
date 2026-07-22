---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: lica.world
  spf: true
hosts:
- cert_expires: Sep 19 14:01:22 2026 GMT
  host: www.lica.world
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Lica
provider_slug: lica
slug: lica-domain-security
source_filename: lica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lica.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 14:01:22 2026 GMT\n  hsts: false\ndomains:\n- domain: lica.world\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lica/refs/heads/main/security/lica-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- B2B
- Artificial Intelligence
- Machine Learning
- Graphic Design
- Generative AI
- Benchmarks
- Datasets
- Model Context Protocol
- Research
---
