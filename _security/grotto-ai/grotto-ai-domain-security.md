---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: grottoai.com
  spf: true
hosts:
- cert_expires: Aug 30 21:21:15 2026 GMT
  host: grottoai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grotto Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grotto AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Grotto AI
provider_slug: grotto-ai
slug: grotto-ai-domain-security
source_filename: grotto-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grottoai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 21:21:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: grottoai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grotto-ai/refs/heads/main/security/grotto-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Multifamily
- Leasing
- Sales Coaching
- PropTech
- Real Estate
- Conversation Intelligence
---
