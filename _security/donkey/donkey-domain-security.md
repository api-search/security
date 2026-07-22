---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: donkey.trade
  spf: true
hosts:
- cert_expires: Sep 30 14:30:39 2026 GMT
  host: donkey.trade
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Donkey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Donkey, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Donkey
provider_slug: donkey
slug: donkey-domain-security
source_filename: donkey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: donkey.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:30:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: donkey.trade\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/donkey/refs/heads/main/security/donkey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Trading
- Logistics
- Supply Chain
- Manufacturing
- Import
- Customs
- Cross-Border
- Y Combinator
- AI
---
