---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kana.ai
  spf: true
hosts:
- cert_expires: Nov  4 23:10:23 2026 GMT
  host: www.kana.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 22:33:37 2026 GMT
  host: apps.kana.ai
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kana, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kana
provider_slug: kana
slug: kana-domain-security
source_filename: kana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kana.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:10:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apps.kana.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 22:33:37 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\ndomains:\n- domain: kana.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kana/refs/heads/main/security/kana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Artificial Intelligence
- Agentic AI
- Marketing Technology
- Audience Intelligence
- Customer Data Platform
- AI Search Optimization
- Growth
---
