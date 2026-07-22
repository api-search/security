---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: perplexity.ai
  spf: true
hosts:
- cert_expires: Sep 15 15:11:24 2026 GMT
  host: www.perplexity.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Comet Browser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Comet
provider_slug: comet-browser
slug: comet-browser-domain-security
source_filename: comet-browser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.perplexity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:11:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: perplexity.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comet-browser/refs/heads/main/security/comet-browser-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Browser
- Consumer
- Agent
- Chromium
- Search
- Perplexity
---
