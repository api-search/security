---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: askwatch.ai
  spf: true
hosts:
- cert_expires: Jan 11 09:24:25 2027 GMT
  host: askwatch.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AskWatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AskWatch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AskWatch
provider_slug: askwatch-ai
slug: askwatch-ai-domain-security
source_filename: askwatch-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: askwatch.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 09:24:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: askwatch.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/askwatch-ai/security/askwatch-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Visibility
- Marketing
- Agencies
- Brand Monitoring
- AI engines
- Autopilot
---
