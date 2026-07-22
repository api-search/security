---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: atomic.ai
  spf: true
hosts:
- cert_expires: Sep 11 19:25:09 2026 GMT
  host: atomic.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atomic Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atomic AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Atomic AI
provider_slug: atomic-ai
slug: atomic-ai-domain-security
source_filename: atomic-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atomic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 19:25:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atomic.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomic-ai/refs/heads/main/security/atomic-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Deep Tech
- Biotechnology
- Drug Discovery
- RNA
- Machine Learning
- Life Sciences
- Artificial Intelligence
---
