---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: infinity.ai
  spf: true
hosts:
- cert_expires: Aug 25 10:20:11 2026 GMT
  host: infinity.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infinity Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infinity AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Infinity AI
provider_slug: infinity-ai
slug: infinity-ai-domain-security
source_filename: infinity-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infinity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:20:11 2026 GMT\n  hsts: null\ndomains:\n- domain: infinity.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infinity-ai/refs/heads/main/security/infinity-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
---
