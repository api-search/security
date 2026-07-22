---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tradelink.co
  spf: true
hosts:
- cert_expires: Sep 30 10:40:20 2026 GMT
  host: en.tradelink.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tradelink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TradeLink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TradeLink
provider_slug: tradelink
slug: tradelink-domain-security
source_filename: tradelink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.tradelink.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:40:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tradelink.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradelink/refs/heads/main/security/tradelink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Supply Chain
- Warehouse Management
- Slot Booking
- Dock and Yard Management
- Collaboration
- SaaS
---
