---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zenquotes.io
  spf: true
hosts:
- cert_expires: Aug 16 19:36:28 2026 GMT
  host: zenquotes.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zen Quotes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zen Quotes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zen Quotes
provider_slug: zen-quotes
slug: zen-quotes-domain-security
source_filename: zen-quotes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zenquotes.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 19:36:28 2026 GMT\n  hsts: false\ndomains:\n- domain: zenquotes.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zen-quotes/refs/heads/main/security/zen-quotes-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Personality
- Public APIs
---
