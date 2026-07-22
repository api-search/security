---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: emmi.ai
  spf: true
hosts:
- cert_expires: Aug 26 22:01:24 2026 GMT
  host: emmi.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emmi Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emmi Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Emmi Ai
provider_slug: emmi-ai
slug: emmi-ai-domain-security
source_filename: emmi-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emmi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 22:01:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: emmi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emmi-ai/refs/heads/main/security/emmi-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Engineering AI
- Physics Simulation
- Machine Learning
- Deep Learning
- Scientific Computing
- CAE
- CFD
- Manufacturing
- Open Source
---
