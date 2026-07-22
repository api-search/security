---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: beesafe.ai
  spf: false
hosts:
- cert_expires: Aug 29 17:50:04 2026 GMT
  host: beesafe.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beesafe Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beesafe Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Beesafe Ai
provider_slug: beesafe-ai
slug: beesafe-ai-domain-security
source_filename: beesafe-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beesafe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 17:50:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: beesafe.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beesafe-ai/refs/heads/main/security/beesafe-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fraud Prevention
- Anti-Scam
- Fraud Detection
- Security
- Artificial Intelligence
- Financial Services
---
