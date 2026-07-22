---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biostate.ai
  spf: true
hosts:
- cert_expires: Oct 15 16:42:10 2026 GMT
  host: biostate.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Biostate Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biostate AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Biostate AI
provider_slug: biostate-ai
slug: biostate-ai-domain-security
source_filename: biostate-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biostate.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 16:42:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: biostate.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biostate-ai/refs/heads/main/security/biostate-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- RNA Sequencing
- Genomics
- Bioinformatics
- Precision Health
- Diagnostics
- Biotechnology
- Machine Learning
---
