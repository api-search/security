---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: newsgurus.ai
  spf: true
hosts:
- cert_expires: Feb 16 16:52:53 2027 GMT
  host: newsgurus.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: News Gurus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for News Gurus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: News Gurus
provider_slug: newsgurus-ai
slug: newsgurus-ai-domain-security
source_filename: newsgurus-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: newsgurus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 16:52:53 2027 GMT\n  hsts: false\ndomains:\n- domain: newsgurus.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/newsgurus-ai/security/newsgurus-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- AI Trading Intelligence
- Market Data
- Trading Signals
- Financial API
- Cryptocurrency
- Commodities
---
