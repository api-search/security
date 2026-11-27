---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ai-advisors.ai
  spf: true
hosts:
- cert_expires: Jan 25 13:56:25 2027 GMT
  host: ai-advisors.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI Advisors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Advisors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AI Advisors
provider_slug: ai-advisors-ai
slug: ai-advisors-ai-domain-security
source_filename: ai-advisors-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai-advisors.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 13:56:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ai-advisors.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ai-advisors-ai/security/ai-advisors-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Marketing
- Software-as-a-Service
- Analytics
- Advertising
- Company
---
