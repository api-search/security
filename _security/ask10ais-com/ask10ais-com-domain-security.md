---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ask10ais.com
  spf: true
hosts:
- cert_expires: Jan 21 11:09:20 2027 GMT
  host: ask10ais.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ask10Ais Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ask10AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ask10AI
provider_slug: ask10ais-com
slug: ask10ais-com-domain-security
source_filename: ask10ais-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ask10ais.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 11:09:20 2027 GMT\n  hsts: false\ndomains:\n- domain: ask10ais.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ask10ais-com/security/ask10ais-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Rankings
- Brand Monitoring
- LLM Evaluation
- AI Visibility
---
