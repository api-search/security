---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kolect.ai
  spf: true
hosts:
- cert_expires: Dec 15 14:34:56 2026 GMT
  host: kolect.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kolect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kolect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kolect
provider_slug: kolect-ai
slug: kolect-ai-domain-security
source_filename: kolect-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kolect.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 14:34:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kolect.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kolect-ai/security/kolect-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Growth Platform
- Paid Media
- Attribution
- AI Insights
---
