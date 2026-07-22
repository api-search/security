---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rebellions.ai
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: rebellions.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rebellions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rebellions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rebellions
provider_slug: rebellions
slug: rebellions-domain-security
source_filename: rebellions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rebellions.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: rebellions.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rebellions/refs/heads/main/security/rebellions-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Tools Infrastructure
- Artificial Intelligence
- AI Inference
- NPU
- Hardware
- Machine Learning
- SDK
- Semiconductors
---
